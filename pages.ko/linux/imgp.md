# imgp

> JPEG 및 PNG 이미지를 위한 커맨드라인 이미지 리사이저 및 회전기.
> 더 많은 정보: <https://github.com/jarun/imgp>.

- 단일 이미지 및/또는 유효한 이미지 형식을 포함한 전체 폴더 변환:

`imgp -x {{1366x1000}} {{경로/대상/폴더}} {{경로/대상/파일}}`

- 이미지를 75% 비율로 조정하고 원본 이미지를 대상 해상도로 덮어쓰기:

`imgp -x {{75}} -w {{경로/대상/파일}}`

- 이미지를 시계 방향으로 90도 회전:

`imgp -o {{90}} {{경로/대상/파일}}`
