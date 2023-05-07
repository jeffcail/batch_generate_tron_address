## batch_generate_tron_address

### 采用go语言实现的可离线断网批量生成波场地址靓号，速度实测每秒可达5000万左右

1. 通过match.txt格式配置需要的靓号， 格式非常简单

2. 速度可配置 -g 配置的协程数量，越高速度越快.  - w 后几位连号

    Mac
   ```vim
   ./batch_generate -g 1000000 -w 4 // 后四位连号
   ./batch_generate -g 1000000 -w 6 // 后6位连号
   ```
   
    windows
    ```cmd
    batch_generate -g 1000000 -w 4 // 后四位连号
    batch_generate -g 1000000 -w 6 // 后6位连号
    ```


3. 符合连号的地址会写进文本文件 如四位靓号，写进 `4位靓号.txt`

4. 文件里带波场地址和私钥

5. 本程序不调用任何外用接口，不将私钥做任何保存

效果:
![avatoar](./4wei.png)