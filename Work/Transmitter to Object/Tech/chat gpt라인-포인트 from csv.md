chat gpt

업로드한 CSV 파일(gaze_x_ref80_px_cal, gaze_y_ref80_px_cal)을 다음 절차로 처리해줘.



1. **데이터 로드**

   - gaze_x_ref80_px_cal, gaze_y_ref80_px_cal 열을 좌표로 사용.

   - n<2이면 스킵.



2. **필터링**

   - 인접 프레임 간 거리(dist = sqrt(dx²+dy²)) 계산.

   - "짧은 구간"만 유지: dist < 30px.

   - 너무 긴 라인 제거:

     - median + 3×IQR 과 95퍼센타일 중 더 작은 값을 임계값으로 설정.

     - dist > 임계값인 선분은 제거.

   - 필터링 없는 원본 버전도 병행 생성.



3. **범위 설정**

   - 전체 범위: (min, max) ± 20px 패딩.

   - 중앙 확대 범위: x,y 각각 20%~80% 분위수 구간.



4. **시각화**

   - (a) 포인트 뷰: 각 좌표를 marker='x', 크기=12px.

   - (b) 라인 뷰: 인접한 좌표를 linewidth=1.8로 연결.

   - 축/눈금/좌표값/배경은 모두 제거, 투명 캔버스.

   - invert_yaxis() 적용(영상 좌표계와 일치).



5. **출력**

   - SVG (확대/인쇄용, 해상도 무관).

   - PNG (투명/흰 배경 필요 시).

   - 각 CSV마다 최소 4종:

     - `_points_all.svg` / `_lines_all.svg` (필터링 없음, 전체)

     - `_points_clean.svg` / `_lines_clean.svg` (튀는 라인 제거, 전체)

     - `_points_zoom.svg` / `_lines_zoom.svg` (필터링 없음, 중앙 확대)

     - `_points_clean_zoom.svg` / `_lines_clean_zoom.svg` (튀는 라인 제거, 중앙 확대)



6. **추가 옵션(필요 시 조정)**

   - DIST_THRESHOLD (짧은 구간 기준, 기본 30px)

   - IQR_K (튀는 라인 제거 강도, 기본 3.0)

   - PCTL_CEIL (95% 기준, 낮출수록 강한 제거)

   - ZOOM_RATIO (기본 30% 범위)

   - POINT_SIZE, LINE_WIDTH (시각 요소)





ㅇ
