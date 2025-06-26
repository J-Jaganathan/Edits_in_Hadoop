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

## 🎁 Bonus

Stay tuned for **RStudio integration** in upcoming parts where I’ll connect Hadoop with powerful analytics tools!

---

## 📜 License

This repository is shared for educational and learning purposes. Feel free to use and modify the configurations as needed.

---

