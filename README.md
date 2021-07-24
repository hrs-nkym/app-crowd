# AWS Amplify & Rekognition Web CAM App

Congestion confirmation

PC の Web カメラで定期的に施設の画像を撮影、画像を 1 秒おきにクラウドに送信、Amazon Rekognition が画像に映った人数をカウントする。
カウント結果を Amazon AppSync でリアルタイムに画面に表示する。

- [React Webcam](https://www.npmjs.com/package/react-webcam)
- [Amazon Rekognition (画像・動画分析)](https://aws.amazon.com/jp/rekognition/?blog-cards.sort-by=item.additionalFields.createdDate&blog-cards.sort-order=desc)
- [AWS ハンズオン](https://aws.amazon.com/jp/builders-flash/202004/crowd-amplify-rekognition/?utm_source=pocket_mylist&awsf.filter-name=*all)

---

## GraphQL Schema

- id: 施設を一意に特定するための ID

- name: 施設の名前

- numberOfPeople: 施設にいる人の数

- description: 施設の説明文

- recordingStatus: モニタリングのカメラが起動中かどうかを示すステータス(ACTIVE / INACTIVE)

---

## Use

```sh
npm start
```

---

## References

[AWS Japan, builders.flash: 日常で楽しむクラウドテクノロジー](https://aws.amazon.com/jp/builders-flash/202004/crowd-amplify-rekognition/?utm_source=pocket_mylist&awsf.filter-name=*all)
