## 사용한 명령어

#### 빌더 추천
```bash
pack builder suggest
```

#### 빌드
```bash
pack build nodejs-app --builder paketobuildpacks/builder-jammy-base
```

#### 실행
```bash
docker run --rm -p 3000:3000 nodejs-app
```

#### 빌드 결과 확인
```bash
curl http://localhost:3000
```



