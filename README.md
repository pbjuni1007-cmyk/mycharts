# mycharts

SKALA 쿠버네티스 실습에서 만든 Helm 차트 저장소입니다. GitHub Pages로 `index.yaml`과 차트 패키지를 그대로 내보냅니다.

| 차트 | 버전 | 내용 |
|---|---|---|
| `sk216-myfirst-chart` | 0.1.0 | 실습용 웹 서버 이미지(`sk216-webserver:1.0.buildkit-pod`)를 띄우는 기본 차트. Deployment, Service, HPA, Ingress 템플릿 포함 |

```bash
helm repo add mycharts https://pbjuni1007-cmyk.github.io/mycharts/
helm search repo mycharts
```

이미지가 실습 환경의 사설 레지스트리에 있어서, 그 밖에서는 설치해도 이미지를 받지 못합니다.
