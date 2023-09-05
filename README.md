<p align="center"> <a href="https://github.com/logpai"> <img src="https://cdn.jsdelivr.net/gh/logpai/logpai.github.io@master/img/logpai_logo.jpg" width="480"></a></p>

# Logparser

<div>
<a href="https://pypi.org/project/logparser3"><img src="https://img.shields.io/badge/python-3.6+-blue" style="max-width: 100%;" alt="Python version"></a>
<a href="https://pypi.org/project/logparser3"><img src="https://img.shields.io/pypi/v/logparser3.svg" style="max-width: 100%;" alt="Pypi version"></a>
<a href="https://github.com/logpai/logparser/actions/workflows/ci.yml"><img src="https://github.com/logpai/logparser/workflows/CI/badge.svg" style="max-width: 100%;" alt="Pypi version"></a>
<a href="https://pepy.tech/project/logparser3"><img src="https://static.pepy.tech/badge/logparser3" style="max-width: 100%;" alt="Downloads"></a>
<a href="https://github.com/logpai/logparser/blob/main/LICENSE"><img src="https://img.shields.io/github/license/logpai/logparser.svg" style="max-width: 100%;" alt="License"></a>
<a href="https://github.com/logpai/logparser#discussion"><img src="https://img.shields.io/badge/chat-wechat-brightgreen?style=flat" style="max-width: 100%;" alt="License"></a>
</div>
<hr/>

<div>
<a href="https://github.com/logpai/logparser/stargazers"><img src="https://reporoster.com/stars/logpai/logparser" /><a/>
</div>

Logparser provides a machine learning toolkit and benchmarks for automated log parsing, which is a crucial step for structured log analytics. By applying logparser, users can automatically extract event templates from unstructured logs and convert raw log messages into a sequence of structured events. The process of log parsing is also known as message template extraction, log key extraction, or log message clustering in the literature.

<p align="center"><img src="https://cdn.jsdelivr.net/gh/logpai/logparser@main/docs/img/example.jpg" width="485"><br>An example of log parsing</p>

### 🌈 New updates

+ Since the first release of logparser, many PRs and issues have been submitted due to incompatibility with Python 3. Finally, we update logparser v1.0.0 with support for Python 3. Thanks for all the contributions! ([#PR86](https://github.com/logpai/logparser/pull/86), [#PR85](https://github.com/logpai/logparser/pull/85), [#PR83](https://github.com/logpai/logparser/pull/83), [#PR80](https://github.com/logpai/logparser/pull/80), [#PR65](https://github.com/logpai/logparser/pull/65), [#PR57](https://github.com/logpai/logparser/pull/57), [#PR53](https://github.com/logpai/logparser/pull/53), [#PR52](https://github.com/logpai/logparser/pull/52), [#PR51](https://github.com/logpai/logparser/pull/51), [#PR49](https://github.com/logpai/logparser/pull/49), [#PR18](https://github.com/logpai/logparser/pull/18), [#PR22](https://github.com/logpai/logparser/pull/22))
+ We build the package wheel logparser3 and release it on pypi. Please install via `pip install logparser3`.
+ We refactor the code structure and beautify the code via the Python code formatter black.

### Log parsers available:

| Publication | Parser | Paper Reference |
| :---: | :---: | :--- |
| IPOM'03 | [SLCT](https://github.com/logpai/logparser/tree/main/logparser/SLCT#slct) | [A Data Clustering Algorithm for Mining Patterns from Event Logs](https://ristov.github.io/publications/slct-ipom03-web.pdf), by Risto Vaarandi. |
| QSIC'08 | [AEL](https://github.com/logpai/logparser/tree/main/logparser/AEL#ael) | [Abstracting Execution Logs to Execution Events for Enterprise Applications](https://www.researchgate.net/publication/4366728_Abstracting_Execution_Logs_to_Execution_Events_for_Enterprise_Applications_Short_Paper), by Zhen Ming Jiang, Ahmed E. Hassan, Parminder Flora, Gilbert Hamann. |
| KDD'09 | [IPLoM](https://github.com/logpai/logparser/tree/main/logparser/IPLoM#iplom) | [Clustering Event Logs Using Iterative Partitioning](https://web.cs.dal.ca/~makanju/publications/paper/kdd09.pdf), by Adetokunbo Makanju, A. Nur Zincir-Heywood, Evangelos E. Milios. |
| ICDM'09 | [LKE](https://github.com/logpai/logparser/tree/main/logparser/LKE#lke) | [Execution Anomaly Detection in Distributed Systems through Unstructured Log Analysis](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/DM790-CR.pdf), by Qiang Fu, Jian-Guang Lou, Yi Wang, Jiang Li. [**Microsoft**]  |
| MSR'10 | [LFA](https://github.com/logpai/logparser/tree/main/logparser/LFA#lfa) | [Abstracting Log Lines to Log Event Types for Mining Software System Logs](http://www.se.rit.edu/~mei/publications/pdfs/Abstracting-Log-Lines-to-Log-Event-Types-for-Mining-Software-System-Logs.pdf), by Meiyappan Nagappan, Mladen A. Vouk. |
| CIKM'11 | [LogSig](https://github.com/logpai/logparser/tree/main/logparser/LogSig#logsig) | [LogSig: Generating System Events from Raw Textual Logs](https://users.cs.fiu.edu/~taoli/pub/liang-cikm2011.pdf), by Liang Tang, Tao Li, Chang-Shing Perng.  |
| SCC'13 | [SHISO](https://github.com/logpai/logparser/tree/main/logparser/SHISO#shiso) | [Incremental Mining of System Log Format](http://ieeexplore.ieee.org/document/6649746/), by Masayoshi Mizutani. |
| CNSM'15 | [LogCluster](https://github.com/logpai/logparser/tree/main/logparser/LogCluster#logcluster) | [LogCluster - A Data Clustering and Pattern Mining Algorithm for Event Logs](http://dl.ifip.org/db/conf/cnsm/cnsm2015/1570161213.pdf), by Risto Vaarandi, Mauno Pihelgas.  |
| CNSM'15 | [LenMa](https://github.com/logpai/logparser/tree/main/logparser/LenMa#lenma) | [Length Matters: Clustering System Log Messages using Length of Words](https://arxiv.org/pdf/1611.03213.pdf), by Keiichi Shima. |
| CIKM'16 | [LogMine](https://github.com/logpai/logparser/tree/main/logparser/LogMine#logmine) | [LogMine: Fast Pattern Recognition for Log Analytics](http://www.cs.unm.edu/~mueen/Papers/LogMine.pdf), by Hossein Hamooni, Biplob Debnath, Jianwu Xu, Hui Zhang, Geoff Jiang, Adbullah Mueen. [**NEC**] |
| ICDM'16 | [Spell](https://github.com/logpai/logparser/tree/main/logparser/Spell#spell) | [Spell: Streaming Parsing of System Event Logs](https://www.cs.utah.edu/~lifeifei/papers/spell.pdf), by Min Du, Feifei Li.  |
| ICWS'17 | [Drain](https://github.com/logpai/logparser/tree/main/logparser/Drain#drain) | [Drain: An Online Log Parsing Approach with Fixed Depth Tree](https://jiemingzhu.github.io/pub/pjhe_icws2017.pdf), by Pinjia He, Jieming Zhu, Zibin Zheng, and Michael R. Lyu.|
| ICPC'18 | [MoLFI](https://github.com/logpai/logparser/tree/main/logparser/MoLFI#molfi) | [A Search-based Approach for Accurate Identification of Log Message Formats](http://publications.uni.lu/bitstream/10993/35286/1/ICPC-2018.pdf), by Salma Messaoudi, Annibale Panichella, Domenico Bianculli, Lionel Briand, Raimondas Sasnauskas.  |

:bulb: Welcome to submit a PR to push your parser code to logparser and add your paper to the table.

### Installation

We recommend installing the logparser package and requirements via pip install.

```
pip install logparser3
```

In particular, the package depends on the following requirements.

+ Python 3.6+
+ regex 2022.3.2
+ numpy
+ pandas
+ scipy
+ scikit-learn
+ deap (if using logparser.MoLFI)
+ nltk (if using logparser.SHISO)
+ gcc (if using logparser.SLCT)
+ perl (if using logparser.LogCluster)

Note that regex matching in Python is brittle, so we recommend fixing the regex library to version 2022.3.2.

### Get started

1. Run the demo:

    For each log parser, we provide a demo to help you get started. Each demo shows the basic usage of a target log parser and the hyper-parameters to configure. For example, the following command shows how to run the demo for Drain.

    ```
    cd logparser/Drain
    python demo.py
    ```
    After finishing running the demo, you can obtain extracted event templates and parsed structured logs in the result folder.

    + [HDFS_2k.log_templates.csv](https://github.com/logpai/logparser/blob/main/logparser/Drain/demo_result/HDFS_2k.log_templates.csv)
    + [HDFS_2k.log_structured.csv](https://github.com/logpai/logparser/blob/main/logparser/Drain/demo_result/HDFS_2k.log_structured.csv)

2. Run the benchmark:
  
    For each log parser, we provide a benchmark script to run log parsing on the [loghub_2k datasets](https://github.com/logpai/logparser/tree/main/data#loghub_2k) for evaluating parsing accuarcy. You can also use [other benchmark datasets for log parsing](https://github.com/logpai/logparser/tree/main/data#datasets).

    ```
    cd logparser/Drain 
    python benchmark.py
    ```

3. Parse your own logs:

    It is easy to apply logparser to parsing your own log data. To do so, you need to install the logparser3 package first. Then you can develop your own script following the below code snippet to start log parsing.

    ```python
    from logparser.Drain import LogParser

    input_dir = 'PATH_TO_LOGS/' # The input directory of log file
    output_dir = 'result/'  # The output directory of parsing results
    log_file = 'unknow.log'  # The input log file name
    log_format = '<Date> <Time> <Level>:<Content>' # Define log format to split message fields
    # Regular expression list for optional preprocessing (default: [])
    regex = [
        r'(/|)([0-9]+\.){3}[0-9]+(:[0-9]+|)(:|)' # IP
    ]
    st = 0.5  # Similarity threshold
    depth = 4  # Depth of all leaf nodes

    parser = LogParser(log_format, indir=input_dir, outdir=output_dir,  depth=depth, st=st, rex=regex)
    parser.parse(log_file)
    ```
    The full example is shown as [example/parse_your_own_logs.py](https://github.com/logpai/logparser/blob/main/example/parse_your_own_logs.py).

### Production use
The main goal of logparser is used for research and benchmark purpose. Researchers can use logparser as a code base to develop new log parsers while practitioners could assess the performance and scalability of current log parsing methods through our benchmarking. We strongly recommend practitioners to try logparser in your production environment. But be aware that the current implementation of logparser is far from ready for production use. Whereas we currently have no plan to do that, we do have a few suggestions for developers who want to build an intelligent production-level log parser.

+ Please be aware of the licenses of [third-party libraries](https://github.com/logpai/logparser/blob/main/THIRD_PARTIES.md) used in logparser. We suggest to keep one parser and delete the others and then re-build the package wheel. This would not break the use of logparser.
+ Please enhance logparser with efficiency and scalability with multi-processing, add failure recovery, add persistence to disk or message queue Kafka.
+ [Drain3](https://github.com/logpai/Drain3) provides a good example for your reference that is built with [practical enhancements] for production scenarios.

### Citation
👋 If you use our logparser tools or benchmarking results in your publication, please cite the following papers.

+ [**ICSE'19**] Jieming Zhu, Shilin He, Jinyang Liu, Pinjia He, Qi Xie, Zibin Zheng, Michael R. Lyu. [Tools and Benchmarks for Automated Log Parsing](https://arxiv.org/pdf/1811.03509.pdf). *International Conference on Software Engineering (ICSE)*, 2019.
+ [**DSN'16**] Pinjia He, Jieming Zhu, Shilin He, Jian Li, Michael R. Lyu. [An Evaluation Study on Log Parsing and Its Use in Log Mining](https://jiemingzhu.github.io/pub/pjhe_dsn2016.pdf). *IEEE/IFIP International Conference on Dependable Systems and Networks (DSN)*, 2016.

### Discussion
Welcome to join our WeChat group for any question and discussion. Alternatively, you can [open an issue here](https://github.com/logpai/logparser/issues/new).

![Scan QR code](https://cdn.jsdelivr.net/gh/logpai/logpai.github.io@master/img/wechat.png)
