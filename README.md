# 📂 Clean Hadoop 3.3.6 Configuration Files (Windows Setup)

Welcome to this repository!
Here you will find **fully working configuration files for Apache Hadoop 3.3.6 on Windows** with complete environment setup and folder structure.

---

## 📋 Included Files

* ✅ `core-site.xml`
* ✅ `hdfs-site.xml`
* ✅ `yarn-site.xml`
* ✅ `mapred-site.xml`
* ✅ `hadoop-env.cmd`
* ✅ `WordCount.java`
* ✅ `MaxMin.java`

These files are tested and verified for a **smooth Hadoop setup with WebUI access** on Windows using Java 8 and winutils.

---

## 📥 Pre-Requisites

* **Apache Hadoop 3.3.6 Binary:**
  [Download from Official Site](https://hadoop.apache.org/releases.html)

* **Java 8 (Adoptium):**
  [Download Here](https://adoptium.net/temurin/releases/?version=8&os=any&arch=any)

* **Winutils for Windows Compatibility:**
  [Download from GitHub](https://github.com/cdarlint/winutils)

* **WinRAR for Smooth Extraction:**
  [Download Here](https://www.win-rar.com/predownload.html?&L=0)

---

## ⚙️ Folder Structure

Ensure you create these directories before running Hadoop:

```text
F:/hadoop/data/namenode
F:/hadoop/data/datanode
```

Provide **full read/write permissions** for all users.

---

## 🚀 Key Commands to Run

```bash
# Format NameNode
hdfs namenode -format

# Start HDFS
start-dfs.cmd

# Start YARN
start-yarn.cmd
```

---

## 🌐 Web UI Access

* **NameNode UI:** [http://localhost:9870](http://localhost:9870)
* **ResourceManager UI:** [http://localhost:8088](http://localhost:8088) or your configured port

---


## 📝 Java Programs Included

### 1. `WordCount.java`  
This is the classic Hadoop MapReduce example for counting word occurrences in a text file.

**Key Concepts:**
- Mapper and Reducer implementation
- Jar compilation with Hadoop classpaths
- Running MapReduce jobs on local HDFS directories
- Input and Output folder setup in HDFS

**Execution Command:**
```bash
hadoop jar WordCount.jar WordCount /WordCount/Input /WordCount/Output
``` 

---

### 2. `MaxMin.java`

This program analyzes real-world weather datasets (NOAA format) to identify **Hot Days** and **Cold Days** based on temperature thresholds.

**Key Concepts:**

- Working with real NOAA datasets 
- Extracting fields using substring operations 
- Conditional filtering for min/max temperatures 
- Processing data using MapReduce logic 

**Execution Command:**

```bash
hadoop jar MaxMin.jar MaxMin /Weather/Input /Weather/Output
```

---

## ⚠️ Disclaimer

This repository is provided **for educational purposes only.**
The programs, configurations, and methods shared here are intended to support learning and experimentation.
The author does not guarantee fitness for any production environment, nor assume responsibility for any misuse, system failure, data loss, or security issues resulting from improper handling.

Note: The Hadoop framework, WordCount algorithm, and MinMax pattern are well-known, community-available examples. This repository shares a curated and tested lab workflow, not proprietary algorithms.

---

## 📜 MIT License

Copyright (c) 2025 Jaganathan J

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

---