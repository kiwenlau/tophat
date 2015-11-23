##1. kiwenlau/tophat镜像

- Base image: Python:2.7
- OS: Debian 8

- tophat	2.0.9
- bowtie2	2.1.0
- samtools	0.1.18

```
sudo docker build  -t kiwenlau/tophat:0.1 .
```

##2. 测试tophat

```
sudo docker run -it kiwenlau/tophat:0.1 bash
```

测试tophat

```
cd test_data
tophat test_ref reads_1.fq reads_2.fq
```
