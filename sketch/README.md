# シモセラ研究室のラフスケッチ線画化アプリケーション
https://esslab.jp/~ess/ja/research/sketch/  
早稲田大学のシモセラ研で行われた深層学習によるラフスケッチ線画化の研究．  
使われてるPytorchのバージョンが古いもので，少し環境構築に手間取った．  
そこで，Dockerを用いた環境構築の方法をここにまとめておく．

# 使い方(sketchディレクトリに入った上で)
git clone https://github.com/bobbens/sketch_simplification.git

docker compose up -d --build

docker compose exec python3 bash

cd sketch_simplification

bash download_models.sh

python simplify.py
