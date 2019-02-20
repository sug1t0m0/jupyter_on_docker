# Dockerで Jupyter Notebook + Keras + TensorFlow 


## 開発に必須
- Docker


## Jupyter Notebookの起動
- Example

```
// イメージのビルド
docker build -t jupyter_example .

// ビルドしたイメージからコンテナを作成
docker run -it --rm -v $PWD:/home/jovyan/work --name jupyter_example -p 8888:8888 jupyter_example
```


- Template

```
// イメージのビルド
docker build -t {イメージ名} .

// ビルドしたイメージからコンテナを作成
docker run -it --rm -v $PWD:/home/jovyan/work --name {コンテナ名} -p 8888:8888 {イメージ名}
```
