# murun-description
뮤런앱 요건정리

## 협업 방식

- Jira
- Swagger UI

## 요구사항

- [x] 곡에 대한 정보는 **아티스트, 타이틀, 곡 uuid, 앨범 이미지 저장경로, 곡 저장경로** 이렇게 주도록 한다.
- [x] ~BPM은 60 ~ 180 사이. 120 == 60 BPM으로 계산하여, 60`~`90범위의 bpm은 그 수를 2배한 BPM디렉터리에도 넣어줘야한다.~
- [x] 120~180범위의 BPM 또한 그 수를 0.5배한 BPM디렉터리에도 넣어줘야한다.
- [x] 곡을 제공할 때에는 기준이 되는 BPM +- 3까지 포함하여 제공한다.
- [x] 곡에 대한 정보에 곡의 길이 (Long) 도 포함하도록 한다. (ex: 3분 00초 -> 180000L)
- [x] bpm이 0일 때, Tobu 의 Higher 를 제공해주도록 한다. (기본 음악)

### 7.7일 업데이트
- [ ] 원본 BPM기준으로 //2 , *2가 들어감. 각각 +-2 ex) 80이 들어온 경우

```text
원본 = 78 79 [80] 81 82
/2 = 38 39 [40] 41 42
*2 = 158 159 [160] 161 162
```
