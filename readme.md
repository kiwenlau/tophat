##1. kiwenlau/tophat镜像

- Base image: Python:2.7
- OS: Debian 8

- tophat	2.0.9
- bowtie2	2.1.0
- samtools	0.1.18

```
sudo docker build  -t kiwenlau/tophat:2.0.9 .
```

##2. 测试tophat

```
sudo docker run -it kiwenlau/tophat:2.0.9 bash
```

测试tophat

```
cd test_data
tophat test_ref reads_1.fq reads_2.fq
cat tophat_out/junctions.bed 
```

```
track name=junctions description="TopHat junctions"
test_chromosome 179 400 JUNC00000001 37 + 179 400 255,0,0 2 71,50 0,171
test_chromosome 350 550 JUNC00000002 37 + 350 550 255,0,0 2 50,50 0,150
```
