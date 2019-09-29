# FIO Benchmark

This project is a [fio](https://github.com/axboe/fio) wrapper written by python.

---

#### Dependency

All dependent packages will be automatically installed by script, but you have to run this script **with root** privileges.

#### How to run

- Perform a full test with default value:

```
bash <(wget -qO- https://github.com/amefs/fio-bench/raw/master/fio-bench.sh -o /dev/null)
```

- Test with options:

  - Test only 1 item (e.g. 4K Q32T1):

  ```
  bash <(wget -qO- https://github.com/amefs/fio-bench/raw/master/fio-bench.sh -o /dev/null) -t 2
  ```

  - Test with larger block

  ```
  bash <(wget -qO- https://github.com/amefs/fio-bench/raw/master/fio-bench.sh -o /dev/null) -s 4g
  ```

  - Test with custom path (default a file under current folder)

  ```
  bash <(wget -qO- https://github.com/amefs/fio-bench/raw/master/fio-bench.sh -o /dev/null) -f /tmp/test.bin
  ```

> **NOTE:** Please make sure you have enough space in your test path!

---

#### 运行依赖

所有依赖都会由脚本自动安装，但必须在 root 权限下运行该脚本。

#### 如何运行

- 使用默认值进行完整基准测试：

```
bash <(wget -qO- https://github.com/amefs/fio-bench/raw/master/fio-bench_zh-cn.sh -o /dev/null)
```

- 附加选项：

  - 仅测试一个项目 (e.g. 4K Q32T1):

  ```
  bash <(wget -qO- https://github.com/amefs/fio-bench/raw/master/fio-bench_zh-cn.sh -o /dev/null) -t 2
  ```

  - 测试更大的数据块 (耗尽高速缓存)

  ```
  bash <(wget -qO- https://github.com/amefs/fio-bench/raw/master/fio-bench_zh-cn.sh -o /dev/null) -s 4g
  ```

  - 在自定义路径测试 (默认在当前文件夹中生成测试文件)

  ```
  bash <(wget -qO- https://github.com/amefs/fio-bench/raw/master/fio-bench_zh-cn.sh -o /dev/null) -f /tmp/test.bin
  ```

> **注意:** 请确保你的测试路径有足够的空间
