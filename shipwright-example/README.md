## 사용한 명령어

### 파이프라인 설치

```bash
kubectl apply -f \
https://storage.googleapis.com/tekton-releases/pipeline/previous/v0.56.0/release.yaml
```

### 십라이트 설치
```bash
kubectl apply -f https://github.com/shipwright-io/build/releases/download/v0.11.0/release.yaml
```

### 빌드 전략 설치
```bash
kubectl apply -f https://github.com/shipwright-io/build/releases/download/v0.11.0/sample-strategies.yaml
```

### Build 객체를 클러스터에 만들기
```bash
kubectl apply -f build-kaniko.yaml
```

### 빌드 실행
```bash
kubectl create -f buildrun.yaml
```

### 로그 확인
```bash
kubectl logs -f kaniko-nodejs-buildrun-b9mmb-qxxxxxx -c step-build-and-push
```

### 빌드 결과 확인
```bash
kubectl get buildrun
```

