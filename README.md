# k8s-home
オンプレミスでデプロイされているKubernetesクラスタを管理しています。
## ハードウェア構成
### 仮想化基盤
以下の3台の仮想基盤サーバでクラスタ構成をとります。
- Intel NUC8i3BEH
  - Intel® Core™ i3-8109U CPU @ 3.60GHz
  - 16GB DDR4
  - 500GB HDD for localdisk
  - VMWare ESXi 7.0.3
- Intel NUC8i5BEH
  - Intel® Core™ i5-8259U CPU @ 3.80GHz
  - 32GB DDR4
  - 1TB HDD for localdisk
  - VMWare ESXi 7.0.3
- Shuttle SH370V2
  - Intel® Core™ i7-9700 CPU @ 3.80GHz
  - 128GB DDR4
  - 500GB HDD for localdisk
  - VMWare ESXi 7.0.3
  
上記の仮想基盤サーバは、以下のストレージを共有ストレージとして利用します。
- QNAP TS-453D
  - 6TB (2TB HDD x 4 RAID5) for storage

## Cluster Components
### Minecraft
マインクラフトサーバには、[MultiPaper](https://github.com/MultiPaper/MultiPaper)を利用しています。
![MultiPaper diagram](diagrams/multipaper-diagram.drawio.svg)
