# hse_hw3_chromhmm
Ссылка на google colab: https://colab.research.google.com/drive/1fuUYGPnh2nC1_5ebxYBTcbu3ldoC1aRK?usp=sharing

Работа производилась для клеточной линии DND-41

### Список 10-ти гистоновых меток (и соотв имен файлов), для которых был сделан анализ

| Гистоновая метка  | Файл |
| ------------- | ------------- |
| H3k27me3 | wgEncodeBroadHistoneDnd41H3k27me3AlnRep1.bam |
| H3k36me3 | wgEncodeBroadHistoneDnd41H3k36me3AlnRep1.bam |
| H3k79me2 | wgEncodeBroadHistoneDnd41H3k79me2AlnRep1.bam |
| H4k20me1 | wgEncodeBroadHistoneDnd41H4k20me1AlnRep1.bam |
| H2az     | wgEncodeBroadHistoneDnd41H2azAlnRep1.bam |
| H3k04me1 | wgEncodeBroadHistoneDnd41H3k04me1AlnRep1.bam |
| H3k04me2 | wgEncodeBroadHistoneDnd41H3k04me2AlnRep1.bam |
| H3k04me3 | wgEncodeBroadHistoneDnd41H3k04me3AlnRep1.bam |
| H3k09ac | wgEncodeBroadHistoneDnd41H3k09acAlnRep1.bam |
| H3k09me3 | wgEncodeBroadHistoneDnd41H3k09me3AlnRep1.bam |
| Control | wgEncodeBroadHistoneDnd41ControlStdAlnRep1.bam |

Файл cellmarkfiletable.txt: https://github.com/cherepasshka/hse_hw3_chromhmm/blob/main/cellmarkfiletable.txt

Папка с выдачей ChromHMM: https://github.com/cherepasshka/hse_hw3_chromhmm/tree/main/modelData

### Картинки из выдачи ChromHMM
![image](https://user-images.githubusercontent.com/50082204/229919009-c7bca8e1-0224-4c59-b376-838e4c1e5a10.png)
![image](https://user-images.githubusercontent.com/50082204/229919098-930d2d6e-32ba-45a3-83f5-dcc617dd0ef8.png)
![image](https://user-images.githubusercontent.com/50082204/229919181-c1feda59-3556-442d-a808-b8bcb8552b8d.png)
![image](https://user-images.githubusercontent.com/50082204/229919290-3447aa6a-ef69-440a-b506-6d08a5a92e12.png)
![image](https://user-images.githubusercontent.com/50082204/229919394-661f3d71-1f35-4de2-8eea-6a8aba36f436.png)


### Табличка с номерами эпигенетических типов, их характерные эпигенетические метки и другие свойства, а также присвоенные им названия
| Номер состояния  | Название | Метки и расположение | Картинка |
| ------------- | ------------- | ------------- | ------------- |
| 1 | Active promoter | <ul><li>для состояния характерны метки H2az, H3k09ac, H3k04me3, H3k04me2, H3k04me1, H3k79me2</li><li>попадает на интрон или экзон</li></ul>|  ![image](https://user-images.githubusercontent.com/50082204/229930803-49ddd079-f2f3-4f11-be45-06aa67ec4221.png) |
| 2 | Weak enhancer | <ul><li>для состояния характерны метки H2az, H3k09ac, H3k04me2, H3k04me1 </li><li>чаще всего находятся на RefSeqTES, RefSeqGene, а также на ядерной ламине</li></ul> | ![image](https://user-images.githubusercontent.com/50082204/229930902-412d065c-837e-477c-999f-a7d183fb4ac5.png) |
| 3 | Weak enhancer | <ul><li>для состояния характерны метки H3k09ac, H3k04me3, H3k04me2, H3k04me1, H3k79me2, H4k20me1, H3k36me3</li><li>проявляется в RefSeqTES, laminB1lads, реже - в RefSeqExon, RefSeqGene, RefSeqTSS2kb</li></ul> | ![image](https://user-images.githubusercontent.com/50082204/229931004-eb0eeca4-38e4-4104-b4fb-b2e8ceaf00fe.png)|
| 4 | Strong enhancer | <ul><li>для состояния характерны метки H3k79me2, H4k20me1, H3k36me3</li><li>чаще всего находятся на RefSeqTES и RefSeqTSS2Kb, а также на ядерной ламине</li></ul> |![image](https://user-images.githubusercontent.com/50082204/229931148-eb00bc68-9d68-4e61-b936-a97c1ec7614a.png)|
| 5 | Transcribed | <ul><li>для состояния характерны метки H3k79me2, H4k20me1, H3k36me3</li><li>проявляется чаще всего в RefSeqGene</li></ul> |![image](https://user-images.githubusercontent.com/50082204/229931314-4c47c379-aaa2-4799-88e6-f123f41acd90.png)|
| 6 | Transcribed | <ul><li>для состояния характерна метка H3k36me3</li><li>проявляется преимущественно в RefSeqExon, RefSeqGene, RefSeqTES</li></ul> | ![image](https://user-images.githubusercontent.com/50082204/229931648-ff2cb29c-c228-4f82-b1ae-a6a16d5e8ff6.png)|
| 7 | Transcribed | <ul><li>для состояния характерна метка H3k36me3</li><li>проявляется преимущественно в RefSeqExon, RefSeqGene, RefSeqTES</li></ul> | ![image](https://user-images.githubusercontent.com/50082204/229931729-bc68377a-25ad-45dc-bb11-726768f70f90.png)|
| 8 | Heterochromatin | <ul><li>для состояния характерны метки H3k36me3 и H3k09me3</li><li>чаще всего находятся на ядерной ламине, попадают на участок репрессированного гетерохроматима</li></ul> | ![image](https://user-images.githubusercontent.com/50082204/229931885-cdeb5f88-ef67-46d8-969e-52d561674e25.png)|
| 9 | Repressed | <ul><li>для состояния ни одна из меток нехарактерна</li><li>чаще всего находятся на ядерной ламине, то есть попадает на участок репрессированного гетерохроматима</li></ul> | ![image](https://user-images.githubusercontent.com/50082204/229931948-0913167f-270c-4774-bf24-780037c92001.png)|
| 10 | Heterochromatin | <ul><li>для состояния характерна метка H3k27me3</li><li>чаще всего находятся на ядерной ламине, то есть попадает на участок репрессированного гетерохроматима</li></ul> |![image](https://user-images.githubusercontent.com/50082204/229932021-f2afff04-fb99-469f-aaaf-b85434a60b8f.png)|


### Список всех запущенных команд:
Установка:
```bash
!curl -O https://raw.githubusercontent.com/deepjavalibrary/d2l-java/master/tools/fix-colab-gpu.sh && bash fix-colab-gpu.sh
!curl -O https://raw.githubusercontent.com/deepjavalibrary/d2l-java/master/tools/colab_build.sh && bash colab_build.sh
!java --list-modules | grep "jdk.jshell"
!wget http://compbio.mit.edu/ChromHMM/ChromHMM.zip
!unzip /content/ChromHMM.zip
```
Скачивание файлов:
```bash
!wget http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneDnd41H3k27me3AlnRep1.bam -O H3k27me3.bam
!wget http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneDnd41H3k36me3AlnRep1.bam -O H3k36me3.bam
!wget http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneDnd41H3k79me2AlnRep1.bam -O H3k79me2.bam
!wget http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneDnd41H4k20me1AlnRep1.bam -O H4k20me1.bam
!wget http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneDnd41H2azAlnRep1.bam -O H2az.bam
!wget http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneDnd41H3k04me1AlnRep1.bam -O H3k04me1.bam
!wget http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneDnd41H3k04me2AlnRep1.bam -O H3k04me2.bam
!wget http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneDnd41H3k04me3AlnRep1.bam -O H3k04me3.bam
!wget http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneDnd41H3k09acAlnRep1.bam -O H3k09ac.bam
!wget http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneDnd41H3k09me3AlnRep1.bam -O H3k09me3.bam! wget http://hgdownload.cse.ucsc.edu/goldenPath/hg19/encodeDCC/wgEncodeBroadHistone/wgEncodeBroadHistoneDnd41ControlStdAlnRep1.bam -O Control.bam
```

Создание cellmarkfiletable.txt:
```python
import os
control = 'Control.bam'
with open(f'cellmarkfiletable.txt', 'a') as f:
  for file in os.listdir():
    name, extension = file.split('.')
    if extension == 'bam' and file != control:
      f.write(f'Dnd41\t{name}\t{file}\t{control}\n')
```

Запуск ChromHMM:
```bash
!java -mx5000M -jar /content/ChromHMM/ChromHMM.jar BinarizeBam -b 200 \
  /content/ChromHMM/CHROMSIZES/hg19.txt /content/ cellmarkfiletable.txt binarizedData
!java -mx5000M -jar /content/ChromHMM/ChromHMM.jar LearnModel -b 200  /content/binarizedData/ /content/modelData/ 10 hg19
```

Бонус:
```python
states = [
    '0_NONE',
    '1_Active_Promoter',
    '2_Weak_Enhancer',
    '3_Weak_Enhancer',
    '4_Strong_Enhancer',
    '5_Transcribed',
    '6_Transcribed',
    '7_Transcribed',
    '8_Heterochromatin',
    '9_Repressed',
    '10_Heterochromatin'
]
lines = []
with open('modelData/Dnd41_10_dense.bed', 'r') as f:
    lines = f.readlines()
for i in range(1, len(lines)):
    tokens = lines[i].split(sep='\t')
    state = int(tokens[3])
    assert(state > 0)
    tokens[3] = states[state]
    lines[i] = '\t'.join(tokens)

with open('Dnd41_10_dense.bed', 'w') as f:
    for line in lines:
        f.write(line)
```
полученный bed файл: https://drive.google.com/file/d/1SdJ6se6QlLPfQVwBHLFywrXkCbUHPF5Y/view?usp=share_link
