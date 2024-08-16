# mycar_for_dev
DonkeyCarの画像認識で走る用コード  
参考：https://docs.donkeycar.com/guide/train_autopilot/  

## DonkeyCarの動かし方
```
cd mycar_for_dev
python manage.py drive
```
ターミナルで起動確認したら、ブラウザの検索バーに
```
<ラズパイのIPアドレス>:8887
```

を入力してenter。

操作画面が出てくるので、適当に動かせるようになる。

IPアドレスはラズパイの小型ディスプレイに表示されている。

## キャリブレーション
[ドキュメント](https://docs.donkeycar.com/guide/train_autopilot/)を参照。

PWMキャリブレーション用コマンド
```
donkey calibrate --channel <your_steering_or_throttle_channel> --bus=<your_i2c_bus>
## steer操作用チャンネル：1  
## throttle操作用チャンネル:0  
## バス番号:1
```