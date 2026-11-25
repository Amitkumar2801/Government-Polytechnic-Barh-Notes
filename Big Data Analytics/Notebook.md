# 📘 CHAMGADAR — BIG DATA ANALYTICS (30 Pages Handwritten Notes)

> **🖊️ 3-Pen Color Guide (Font: Panton Arabic Semi Bold):**
> - **⬛ BLACK PEN:** Headings & Subheadings
> - **🟦 BLUE PEN:** Simple English Explanations & Real-Life Examples
> - **🟥 RED PEN:** Definitions, `★ IMP` Points, Formulas & Conclusions
> - **🖍️ HIGHLIGHTER:** Key Exam Words

---

## 📋 STUDENT DETAILS

| Field | Details |
|:---:|:---:|
| **Name** | AMIT KUMAR |
| **Course** | Artificial Intelligence & Machine Learning |
| **Semester** | 5th |
| **Roll No.** | 49 |

---

## 📑 INDEX (30 PAGES)

| Unit No. | Topic Name | Page No. |
|:--------:|:-----------|:--------:|
| Unit 1.1 | Introduction of Big Data, 5 Vs, Processing & Tools | 1 - 3 |
| Unit 1.2 | Basics of Big Data (Data Types, Scaling & 4 Analytics) | 4 - 6 |
| Unit 1.3 | Significance of Big Data (Industries & AI/ML) | 7 |
| Unit 2.1 | Introduction of Hadoop (History, Features & Data Locality) | 8 |
| Unit 2.2 | Hadoop Ecosystem Overview | 9 |
| Unit 2.3 | HDFS Architecture, Replication & Fault Tolerance | 10 - 12 |
| Unit 2.4 | Hadoop Architecture (YARN, HDFS, MapReduce) | 13 |
| Unit 2.5 | MapReduce (Phases, Mapper/Reducer & Job Anatomy) | 14 - 15 |
| Unit 3.1 | Introduction to NoSQL (Definition & Applications) | 16 |
| Unit 3.2 | Types of NoSQL Databases (4 Types) | 17 - 18 |
| Unit 3.3 - 3.4 | Advantages of NoSQL & Use in Industry | 19 |
| Unit 3.5 - 3.7 | SQL vs NoSQL vs NewSQL | 20 |
| Unit 3 (Lab) | Creating Indexes for Engineering Data | 21 |
| Unit 3 (Lab) | Exploratory Data Analysis (EDA) in Python | 22 |
| Unit 3 (Theory) | Functional Dependency, Trivial/Non-Trivial, Closure ($F^+$, $X^+$) | 23 |
| Unit 4.1 | Introduction to MongoDB, RDBMS Comparison & Use Cases | 24 - 25 |
| Unit 4.2 | MongoDB Data Model (BSON & Engineering Schema) | 25 - 26 |
| Unit 4.3 | CRUD Operations in MongoDB Shell | 27 - 28 |
| Unit 4.4 | Data Modeling Best Practices & Indexing | 29 - 30 |

---

## 📄 PAGE 1 — UNIT 1.1: INTRODUCTION OF BIG DATA

### ⬛ Q. What is Big Data? Explain with Traditional Data Comparison. *(4/6 Marks)*
> 🟥 **Definition:** **Big Data** refers to **extremely large, fast-moving, and complex datasets** that traditional data software (like MS Excel or single-server MySQL) cannot store, manage, or process within a reasonable time.

### ⬛ Detailed Explanation & Real-Life Examples
- 🟦 **Why Traditional Tools Fail:** Traditional systems handle Gigabytes (GB) in neat rows & columns on one machine. Today, apps generate Terabytes (TB) and Petabytes (PB) of mixed data every minute.
- 🟦 **Student Example:** Storing attendance of 60 students in your college Excel sheet is **Traditional Data**.
- 🟦 **Company Example:** Instagram users uploading 65,000+ photos/minute, Zomato tracking lakhs of live orders, and YouTube streaming millions of HD videos is **Big Data**.

| Feature | Traditional Data | Big Data |
|:--------|:-----------------|:---------|
| **Volume** | MB to GB | **TB to PB & Exabytes** |
| **Format** | Only Structured (Tables) | **Structured + JSON + Videos/Images** |
| **Speed** | Slow / Batch updates | **Very Fast / Real-time streaming** |
| **Storage** | 1 Computer / Server | **Distributed Cluster (Many PCs)** |

### ⬛ 2D Architecture Diagram
```text
  TRADITIONAL (1 PC)                 BIG DATA (Distributed Cluster)
  +--------------+                   +------+   +------+   +------+
  | Excel / SQL  |                   | PC 1 |---| PC 2 |---| PC 3 |
  | (GB, Tables) |                   +------+   +------+   +------+
  +--------------+                    (TB/PB, Mixed Formats, Fast)
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Handles massive scale, uncovers hidden business trends, powers AI/ML.
- ❌ **Disadvantages:** Needs costly infrastructure/clusters, skilled engineers, and strong privacy security.

> 🟥 **Conclusion:** Big Data turns massive raw information into actionable insights where traditional databases fail.

---

## 📄 PAGE 2 — UNIT 1.1: KEY CHARACTERISTICS (THE 5 Vs OF BIG DATA)

### ⬛ Q. Explain the 5 Vs of Big Data with Real-Life Examples. *(6 Marks ★ Very Imp)*
> 🟥 **Definition:** The **5 Vs of Big Data** — **Volume, Velocity, Variety, Veracity, and Value** — are the five core characteristics that define and distinguish Big Data from normal data.

### ⬛ Detailed Explanation of Each V
1. **Volume (Size):** Huge amount of data generated every second (Terabytes to Petabytes). *Ex:* Facebook & YouTube store petabytes of daily photos and videos.
2. **Velocity (Speed):** Fast speed at which data arrives and needs instant processing. *Ex:* Google Maps live traffic and UPI/credit card fraud checks in <1 second.
3. **Variety (Formats):** Data arrives in multiple shapes — **Structured** (SQL tables), **Semi-Structured** (JSON/XML), and **Unstructured** (images, audio, CCTV).
4. **Veracity (Accuracy & Trust):** Quality and reliability of data. *Ex:* Removing fake bot reviews and faulty IoT sensor readings before analysis.
5. **Value (Usefulness):** Extracting real business profit or insights from data. *Ex:* Netflix recommending movies users actually watch.

### ⬛ 2D Star Diagram (The 5 Vs)
```text
                      [ 1. VOLUME (Size: TB/PB) ]
                                  |
  [ 5. VALUE (Profit) ] ----------+---------- [ 2. VELOCITY (Live Speed) ]
                                 / \
       [ 4. VERACITY (Trust) ]--+   +--[ 3. VARIETY (Mixed Formats) ]
```

### ⬛ Advantages & Disadvantages of Understanding 5 Vs
- ✅ **Advantages:** Helps engineers choose the right storage (HDFS/NoSQL) and processing engine (Spark/Kafka).
- ❌ **Disadvantages:** Managing all 5 Vs simultaneously (especially high Velocity + Veracity) increases system complexity.

> 🟥 **Conclusion:** Without **Value** and **Veracity**, massive **Volume**, **Velocity**, and **Variety** are useless noise.

---

## 📄 PAGE 3 — UNIT 1.1: BIG DATA PROCESSING & COMMON TOOLS

### ⬛ Q. How Is Big Data Processed? Explain Common Big Data Tools. *(6 Marks)*
> 🟥 **Definition:** **Big Data Processing** is a multi-stage workflow that collects raw datasets from diverse sources, stores them across distributed clusters, and runs analytics to produce visual insights.

### ⬛ 3 Stages of Big Data Processing (Workflow)
1. **Integration (Collection):** Collecting and combining raw data from mobile apps, IoT sensors, server logs, and SQL databases into one pipeline (*Ex:* Swiggy combining app clicks + GPS + order DB).
2. **Storage & Management:** Splitting and storing huge mixed datasets across distributed servers or Cloud Data Lakes (*Ex:* Hadoop HDFS, Amazon S3).
3. **Analysis & Visualization:** Running batch/real-time queries, ML models, and dashboards (*Ex:* Power BI/Tableau live sales graphs).

### ⬛ Workflow Diagram
```text
  [Sources: Apps, IoT] --> [1. Integration] --> [2. Storage (HDFS/Cloud)] --> [3. Analysis & Dashboards]
```

### ⬛ Common Big Data Tools & Concepts
| Tool / Concept | Role & Simple Explanation |
|:---------------|:--------------------------|
| **Apache Hadoop** | Distributed storage (**HDFS**) + batch processing (**MapReduce**) framework. |
| **Apache Spark** | **100x faster** in-memory distributed processing engine for batch, streaming & ML. |
| **Apache Kafka** | High-throughput platform for **real-time live event streaming**. |
| **NoSQL & Data Lakes** | Flexible storage (MongoDB, Cassandra, S3) for raw, varied, large-scale data. |

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Parallel execution saves hours of time; supports both live streaming and batch reports.
- ❌ **Disadvantages:** Integrating multiple tools (Kafka + Spark + HDFS) requires skilled Data Engineers.

> 🟥 **Conclusion:** Tools like Hadoop, Spark, and Kafka form the backbone of modern Big Data pipelines.

---

## 📄 PAGE 4 — UNIT 1.2: BASICS OF BIG DATA (3 TYPES OF DATA)

### ⬛ Q. Explain Structured, Semi-Structured & Unstructured Data. *(4/6 Marks)*
> 🟥 **Definition:** **Data Classification** divides Big Data into three categories based on whether it follows a fixed table schema or not: **Structured, Semi-Structured, and Unstructured**.

### ⬛ Detailed Explanation & Real-Life Examples
1. **Structured Data (~10–15%):** Strictly organized in rows & columns (fixed schema). Easy to search using SQL.
   - *Student Ex:* College Exam Result Table (`Roll_No | Name | Marks`). *Company Ex:* Bank transactions in MySQL.
2. **Semi-Structured Data (~5–10%):** No fixed table, but uses **tags or key-value pairs** (`{key: value}`).
   - *Company Ex:* Zomato/Amazon order receipt stored in **JSON** or **XML** format.
3. **Unstructured Data (~75–80%):** No predefined structure or schema. Hardest to search without AI/NLP.
   - *Real Ex:* WhatsApp voice messages, Instagram Reels, CCTV videos, PDFs, Tweets.

| Feature | Structured | Semi-Structured | Unstructured |
|:--------|:-----------|:----------------|:-------------|
| **Schema** | Fixed & Strict | Flexible (Tags/Keys) | No Schema |
| **Storage** | RDBMS (MySQL) | NoSQL (MongoDB) | HDFS / Data Lakes |
| **Searchability** | Very Easy (SQL) | Moderate | Hard (Needs AI/ML) |

### ⬛ 2D Classification Diagram
```text
                         [ TYPES OF BIG DATA ]
            +----------------------+----------------------+
            v                      v                      v
  [Structured (SQL)]    [Semi-Structured (JSON)]    [Unstructured (Video)]
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Knowing the data type helps pick the fastest storage (SQL vs MongoDB vs Data Lake).
- ❌ **Disadvantages:** Unstructured data (~80%) consumes massive storage and needs heavy AI/ML to extract value.

> 🟥 **Conclusion:** Big Data systems are specifically built to handle the ~80% unstructured and semi-structured data that RDBMS ignores.

---

## 📄 PAGE 5 — UNIT 1.2: ARCHITECTURE LAYERS & SCALING

### ⬛ Q. Explain Big Data Architecture & Vertical vs. Horizontal Scaling. *(6 Marks)*
> 🟥 **Definition:** **Big Data Architecture** is a layered blueprint for ingesting, storing, processing, and visualizing massive datasets, while **Scaling** increases system capacity to handle growth.

### ⬛ 5 Layers of Big Data Architecture
1. **Sources Layer:** Apps, IoT sensors, social media, web logs.
2. **Ingestion Layer:** Pulls data in (Batch: Sqoop | Streaming: Kafka).
3. **Storage Layer:** Distributed files & DBs (HDFS, Amazon S3, NoSQL).
4. **Processing Layer:** Parallel compute engines (MapReduce, Spark).
5. **Analytics Layer:** ML models, SQL, Power BI / Tableau dashboards.

### ⬛ Vertical Scaling vs. Horizontal Scaling
| Feature | Vertical Scaling (Scale-Up) | Horizontal Scaling (Scale-Out) |
|:--------|:----------------------------|:-------------------------------|
| **Meaning** | Add more **RAM/CPU to 1 PC** | Add **more PCs (nodes)** to cluster |
| **Cost & Limit** | Expensive; hardware limit | Cost-effective; **unlimited scale** |
| **Fault Tolerance** | Low (1 server fails = down) | **High** (other PCs keep running) |

### ⬛ 2D Scaling Diagram
```text
  VERTICAL (Scale-Up)               HORIZONTAL (Scale-Out)
   +---------------+                +------+   +------+   +------+
   | 1 BIG SERVER  |                | PC 1 |---| PC 2 |---| PC 3 |
   | (++RAM/++CPU) |                +------+   +------+   +------+
   +---------------+                  (Distributed Big Data Cluster)
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages (Horizontal):** No single point of failure, cheap commodity servers, easy expansion.
- ❌ **Disadvantages:** Distributed clusters require network coordination and careful cluster management.

> 🟥 **Conclusion:** Big Data relies on **Horizontal Scaling** across layered architectures to grow reliably at low cost.

---

## 📄 PAGE 6 — UNIT 1.2: 4 TYPES OF BIG DATA ANALYTICS

### ⬛ Q. Explain the 4 Types of Big Data Analytics with Real Examples. *(6 Marks)*
> 🟥 **Definition:** **Big Data Analytics** is classified into **4 progressive levels** — Descriptive, Diagnostic, Predictive, and Prescriptive — moving from understanding the past to automating future decisions.

### ⬛ Detailed Explanation (Real Company Example: Flipkart)
1. **Descriptive Analytics (*"What happened?"*):** Summarizes past data into reports & charts.
   - *Flipkart Ex:* "Today we received 50,000 orders worth ₹4 Crore."
2. **Diagnostic Analytics (*"Why did it happen?"*):** Finds the root cause of an event.
   - *Flipkart Ex:* "Orders dropped 15% between 2–4 PM because the UPI gateway was down."
3. **Predictive Analytics (*"What will happen?"*):** Uses Machine Learning to forecast future trends.
   - *Flipkart Ex:* "Smartphone sales will jump 40% during next month's Big Billion Sale."
4. **Prescriptive Analytics (*"What should we do?"*):** Recommends the best action to take.
   - *Flipkart Ex:* "Pre-stock 10,000 extra phones in Patna & Delhi warehouses to deliver in 1 day!"

### ⬛ 2D Workflow Diagram
```text
  [1. Descriptive] ---> [2. Diagnostic] ---> [3. Predictive] ---> [4. Prescriptive]
  (What happened?)      (Why happened?)      (What next?)         (Best Action!)
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Turns raw history into smart future strategies, reduces losses, increases profit.
- ❌ **Disadvantages:** Predictive & Prescriptive analytics need clean historical data and advanced ML models.

> 🟥 **Conclusion:** Moving from Descriptive to Prescriptive analytics gives organizations maximum competitive advantage.

---

## 📄 PAGE 7 — UNIT 1.3: SIGNIFICANCE OF BIG DATA

### ⬛ Q. Explain the Significance of Big Data Across Industries. *(6 Marks)*
> 🟥 **Definition:** **Significance of Big Data** refers to the **strategic value and transformative impact** of analytics on business decisions, cost savings, AI innovation, and society. Data is called the **"New Oil"**.

### ⬛ 5 Core Pillars & Industry Applications
1. **Smart & Fast Decisions:** Airlines dynamically adjust ticket prices based on live seat demand.
2. **Personalization:** Netflix, Spotify & Amazon tailor recommendations to each user's taste.
3. **Fraud & Risk Control:** Banks/UPI apps analyze millions of transactions per second to block fraud in <1s.
4. **Healthcare & Life Saving:** Hospitals use AI on MRI/X-ray Big Data to detect cancer & outbreaks early.
5. **Fuel for AI & ML:** ChatGPT, self-driving cars, and robotics require massive datasets to achieve high accuracy.

| Industry | Significance & Real-World Example |
|:---------|:----------------------------------|
| **Healthcare** | Early disease detection, genomics, personalized medicine. |
| **Banking** | Instant credit card / UPI fraud detection & loan risk scoring. |
| **Smart Cities** | Google Maps live traffic routing & smart electricity grids. |
| **Education** | Tracking student progress on NPTEL/Coursera & reducing dropouts. |

### ⬛ 2D Hub Diagram
```text
               [ Smart Decisions ]
                        |
  [ Cost Saving ] ------+------ [ Personalization ]
                 ( BIG DATA )
  [ Fraud Stop ] -------+------ [ AI / ML Fuel ]
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Beats competitors, saves lives, cuts operational waste, powers AI.
- ❌ **Disadvantages:** User privacy risks, high data-center power consumption, data-quality bias.

> 🟥 **Conclusion:** Big Data is the "New Oil" driving Industry 4.0, modern AI, and smarter public services.

---

## 📄 PAGE 8 — UNIT 2.1: INTRODUCTION OF HADOOP

### ⬛ Q. What is Apache Hadoop? Explain its History, Features & Data Locality. *(6 Marks)*
> 🟥 **Definition:** **Apache Hadoop** is an **open-source, Java-based distributed computing framework** that stores and processes massive datasets across clusters of inexpensive, ordinary (commodity) computers.

### ⬛ History & Origin Story
- **2003–2004:** Google published **GFS** (storage) and **MapReduce** (processing) papers.
- **2006:** **Doug Cutting** and **Mike Cafarella** separated these modules from Apache Nutch and named the project **Hadoop** (after Doug's son's **yellow toy elephant**).

### ⬛ Key Features of Hadoop
1. **Open Source & Economical:** Free software running on low-cost commodity PCs.
2. **Fault-Tolerant:** Automatically keeps **3 replicas** of every data block.
3. **Horizontal Scalability:** Add thousands of nodes without stopping the cluster.
4. **Data Locality *(★ Imp)*:** Sends the **program code to the node where the data already lives**, avoiding slow network transfers!

### ⬛ 2D Data Locality Diagram
```text
  OLD WAY (Slow):  [Huge Data] =====(Heavy Network Transfer)=====> [Compute PC]
  HADOOP (Fast):   [Data Block + Compute Program on SAME Node]  (Zero Delay!)
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Stores any format (text, video, logs), fault-tolerant, cheap, massively scalable.
- ❌ **Disadvantages:** High overhead for small files, batch-oriented (slower than Spark for live streams), basic default security.

> 🟥 **Conclusion:** Hadoop revolutionized Big Data by making petabyte-scale computing affordable on ordinary hardware.

---

## 📄 PAGE 9 — UNIT 2.2: HADOOP ECOSYSTEM OVERVIEW

### ⬛ Q. Explain the Hadoop Ecosystem and its Core Components. *(6 Marks)*
> 🟥 **Definition:** The **Hadoop Ecosystem** is a **suite of open-source tools and frameworks** built around core Hadoop to support data ingestion, storage, resource management, processing, and querying.

### ⬛ Core & Ecosystem Components
| Component | Category | Function & Real-World Use |
|:----------|:---------|:--------------------------|
| **HDFS** | Storage | Splits & stores big files across cluster nodes (128 MB blocks). |
| **YARN** | Resource Manager | Allocates CPU & RAM and schedules jobs across cluster nodes. |
| **MapReduce** | Batch Processing | Processes massive datasets in parallel using Map & Reduce. |
| **Apache Hive** | Data Warehouse | Runs **SQL-like queries (HiveQL)** on HDFS without Java code. |
| **Apache Pig** | ETL Scripting | Uses **Pig Latin** scripts to clean & transform raw data. |
| **Apache HBase** | NoSQL DB | Column-oriented DB on HDFS for **fast random read/write**. |
| **Sqoop / Flume** | Data Ingestion | **Sqoop:** RDBMS ↔ HDFS | **Flume:** Streams server/social logs. |
| **Apache Spark** | Fast Engine | In-memory distributed engine (**100x faster** than MapReduce). |

### ⬛ Layered Architecture Diagram
```text
+-------------------------------------------------------------------+
|  ANALYTICS & ML:  [ Hive (SQL) ]   [ Pig (ETL) ]   [ Spark ML ]   |
+-------------------------------------------------------------------+
|  INGESTION:       [ Sqoop (MySQL <-> HDFS) ]   [ Flume (Logs) ]   |
+-------------------------------------------------------------------+
|  PROCESSING:      [ MapReduce (Batch) ]   [ Apache Spark (Fast) ] |
+-------------------------------------------------------------------+
|  RESOURCE MGMT:   [ YARN (ResourceManager & NodeManager) ]        |
+-------------------------------------------------------------------+
|  STORAGE:         [ HDFS (Distributed Files) ]   [ HBase ]        |
+-------------------------------------------------------------------+
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** One ecosystem covers everything from SQL (Hive) to streaming (Flume/Spark) and storage (HDFS).
- ❌ **Disadvantages:** Complex to configure, monitor, and maintain many different tools together.

> 🟥 **Conclusion:** The Hadoop Ecosystem turns core Hadoop into a complete end-to-end Big Data platform.

---

## 📄 PAGE 10 — UNIT 2.3: HDFS BASICS & ARCHITECTURE

### ⬛ Q. What is HDFS? Explain NameNode and DataNode Architecture. *(6 Marks)*
> 🟥 **Definition:** **HDFS (Hadoop Distributed File System)** is the **primary distributed storage system** of Hadoop that splits very large files into **128 MB blocks** and stores them across clusters using a **Master-Slave** architecture.

### ⬛ Key Features & NameNode vs. DataNode
- **Write-Once, Read-Many (WORM):** Optimized for high-throughput batch reads.
- **Real Example:** Storing 50 TB of CCTV / satellite videos split into 128 MB chunks across 100 servers.

| Feature | NameNode (Master) | DataNode (Slave / Worker) |
|:--------|:------------------|:--------------------------|
| **Primary Job** | Stores **Metadata** (file names, block map) | Stores **actual 128 MB data blocks** |
| **Storage Medium** | Kept in **RAM** for fast lookup | Stored on **Hard Disks** |
| **Key Files** | **`FsImage`** (snapshot) + **`EditLogs`** (log) | Raw block files + Checksums |
| **Heartbeat** | Receives heartbeats from all DataNodes | Sends **Heartbeat every 3 seconds** |

### ⬛ 2D HDFS Architecture Diagram
```text
                    +-------------------------+
                    |    NameNode (Master)    | (Metadata: FsImage + EditLogs)
                    +-----+-------------+-----+
           Heartbeat (3s) |             | Block Commands
                          v             v
  [Client] ---------> [DataNode 1]  [DataNode 2]  [DataNode 3]
  (Read/Write)        [B1] [B2]     [B1] [B3]     [B2] [B3]
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Stores petabytes cheaply, high streaming throughput, handles hardware failure automatically.
- ❌ **Disadvantages:** Poor for storing millions of tiny (<1 MB) files (fills NameNode RAM); not for random low-latency writes.

> 🟥 **Conclusion:** HDFS provides reliable, scalable storage by separating Metadata (NameNode) from Data Blocks (DataNodes).

---

## 📄 PAGE 11 — UNIT 2.3: HDFS STORING, REPLICATION & RACK AWARENESS

### ⬛ Q. Explain File Storing, Replication & Rack Awareness in HDFS. *(4/6 Marks)*
> 🟥 **Definition:** **HDFS Replication** is the process of automatically saving multiple copies (**Default Replication Factor = 3**) of each data block across different nodes and server racks for safety.

### ⬛ Step-by-Step Storing & Replication Process
1. **File Splitting:** Suppose a student uploads a **300 MB** video dataset. With 128 MB block size, HDFS splits it into **3 blocks**: `B1 (128 MB)`, `B2 (128 MB)`, `B3 (44 MB)`.
2. **Metadata Check:** Client asks **NameNode** where to write. NameNode gives addresses of 3 DataNodes.
3. **Write Pipeline:** Client writes `B1` to **DN1** → DN1 forwards a copy to **DN2** → DN2 forwards a copy to **DN3**.
4. **Rack Awareness Policy:**
   - **Copy 1:** Placed on local **Rack 1**.
   - **Copy 2:** Placed on a **different rack (Rack 2)** (protects against full rack power/switch failure).
   - **Copy 3:** Placed on a **different node inside Rack 2** (saves cross-rack bandwidth).

### ⬛ 2D Replication & Rack Awareness Diagram
```text
  [300 MB File] --> Split: [B1: 128MB] [B2: 128MB] [B3: 44MB]

  [Client] ---> [Rack 1: DN1 (Copy 1)] ===> [Rack 2: DN2 (Copy 2)] ===> [Rack 2: DN3 (Copy 3)]
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Even if an entire server rack loses electricity, 2 copies remain safe on another rack; enables fast parallel reads.
- ❌ **Disadvantages:** 3x replication uses **3x disk space** (300 MB file uses 900 MB total raw disk).

> 🟥 **Conclusion:** Rack-aware 3x replication makes HDFS virtually immune to single-disk or single-rack failures.

---

## 📄 PAGE 12 — UNIT 2.3: HDFS FAULT TOLERANCE & DATA RECOVERY

### ⬛ Q. Explain Fault Tolerance and Data Recovery Mechanisms in HDFS. *(6 Marks)*
> 🟥 **Definition:** **Fault Tolerance** is HDFS's ability to **continue operating smoothly without data loss** even when one or more DataNodes or disks crash.

### ⬛ 5 Fault Tolerance Mechanisms
1. **Heartbeat & Dead-Node Detection:** Every DataNode sends a **Heartbeat every 3 seconds** to the NameNode. If no heartbeat arrives for **10 minutes**, NameNode marks that DataNode **Dead**.
2. **Automatic Re-Replication:** When a DataNode dies, NameNode sees block replication dropped from `3` to `2` and immediately orders healthy nodes to copy missing blocks to other healthy DataNodes.
3. **Rack Awareness:** Stores replicas across at least 2 racks so rack failures do not destroy data.
4. **Checksum Verification:** HDFS checks data integrity using checksums during reads; if corrupted, it fetches a clean replica.
5. **Secondary NameNode & Safe Mode:** Secondary NameNode periodically merges `FsImage + EditLogs` (checkpointing) for fast NameNode recovery.

### ⬛ 2D Crash & Recovery Diagram
```text
  1. NORMAL:     DN1 [B1]       DN2 [B1]       DN3 [B1]     (Replication = 3)
                                    |
  2. CRASH!:                   (DN2 CRASHES!) -> No Heartbeat (10m) -> Marked DEAD
                                    v
  3. RECOVERY:   NameNode orders DN1 ---(copy [B1])---> DN4 [B1]  (3x Restored!)
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Zero manual intervention needed during node crashes; automatic self-healing cluster.
- ❌ **Disadvantages:** Re-replicating terabytes after a huge node crash temporarily consumes heavy network bandwidth.

> 🟥 **Conclusion:** Heartbeats, checksums, and automatic re-replication make HDFS one of the most fault-tolerant storage systems.

---

## 📄 PAGE 13 — UNIT 2.4: HADOOP ARCHITECTURE (YARN + HDFS)

### ⬛ Q. Explain Hadoop Architecture & Compare Hadoop 1.0 vs. 2.0/3.0. *(6 Marks)*
> 🟥 **Definition:** **Hadoop Architecture** is a **layered Master-Slave framework** combining **HDFS** (Storage), **YARN** (Resource Management), and **MapReduce** (Processing) to run parallel applications reliably.

### ⬛ Core Layers & YARN Components
1. **HDFS Layer:** NameNode (Master) + DataNodes (Slaves) for distributed file storage.
2. **YARN Layer (Yet Another Resource Negotiator):**
   - **ResourceManager (Master):** Global scheduler allocating CPU & RAM across all jobs.
   - **NodeManager (Slave):** Runs on each node, manages **Containers**, and monitors RAM/CPU.
   - **ApplicationMaster:** Created per job to negotiate containers and track task progress.
3. **Processing Layer:** Executes MapReduce, Spark, or Tez inside YARN Containers.

| Feature | Hadoop 1.0 | Hadoop 2.0 / 3.0 |
|:--------|:-----------|:-----------------|
| **Resource Manager** | JobTracker (Single bottleneck) | **YARN (ResourceManager + AppMaster)** |
| **Processing Engines** | Only Batch (MapReduce) | **Batch + Streaming + Graph (Spark, Tez)** |
| **NameNode HA** | Single Point of Failure | **High Availability (Active + Standby)** |

### ⬛ 2D Architecture Diagram
```text
  +---------------------------------------------------------------+
  |  PROCESSING:  [ MapReduce ]      [ Apache Spark ]  [ Hive ]   |
  +---------------------------------------------------------------+
  |  YARN LAYER:  [ ResourceManager ] ---> [ AppMaster ]          |
  |                   |                         |                 |
  |               [ NodeManager + Containers on Worker Nodes ]    |
  +---------------------------------------------------------------+
  |  HDFS LAYER:  [ NameNode ] ---> [ DataNode 1 ] [ DataNode 2 ] |
  +---------------------------------------------------------------+
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** YARN lets Hadoop run Spark, Hive, and MapReduce simultaneously on the same cluster (high utilization).
- ❌ **Disadvantages:** YARN adds architectural complexity with multiple daemons to tune and monitor.

> 🟥 **Conclusion:** Separating YARN from MapReduce in Hadoop 2.0/3.0 transformed Hadoop into a multi-engine Big Data OS.

---

## 📄 PAGE 14 — UNIT 2.5: MAPREDUCE PHASES & WORDCOUNT EXAMPLE

### ⬛ Q. What is MapReduce? Explain All Phases with WordCount Example. *(6 Marks ★ Imp)*
> 🟥 **Definition:** **MapReduce** is a **distributed programming model** in Hadoop that processes massive datasets in parallel using two core functions: **Map()** (filter/transform) and **Reduce()** (aggregate/summarize).

### ⬛ 6 Phases of MapReduce (Workflow)
1. **Input Splits:** Divides large input file into logical chunks (typically 128 MB each).
2. **RecordReader:** Converts each split into `<Key, Value>` pairs (e.g., `<LineOffset, LineText>`).
3. **Map Phase:** **Mapper** processes each input record and outputs intermediate `<Key, Value>` pairs.
4. **Shuffle & Sort:** Groups all values having the same key and sorts keys alphabetically.
5. **Reduce Phase:** **Reducer** aggregates the grouped values for each key (sum, count, average).
6. **OutputFormat:** Writes the final `<Key, Value>` output files permanently to **HDFS**.

### ⬛ 2D WordCount Workflow Diagram
```text
  INPUT: "Big Data\nBig AI"
     +--> [Split 1] --> MAP --> ("Big",1), ("Data",1)
     +--> [Split 2] --> MAP --> ("Big",1), ("AI",1)
                            |
                     [SHUFFLE & SORT] --> ("AI",[1]), ("Big",[1,1]), ("Data",[1])
                            |
                        [REDUCER] ------> ("AI",1), ("Big",2), ("Data",1) [HDFS]
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Simple parallel logic, automatic fault recovery, scales easily to petabytes.
- ❌ **Disadvantages:** Slow for iterative ML/real-time jobs because it writes intermediate data to disk after every step.

> 🟥 **Conclusion:** MapReduce simplifies parallel Big Data programming by automating splitting, shuffling, and fault recovery.

---

## 📄 PAGE 15 — UNIT 2.5: MAPPER VS. REDUCER & JOB ANATOMY

### ⬛ Q. Compare Mapper vs. Reducer & Explain MapReduce Job Anatomy. *(6 Marks)*
> 🟥 **Definition:** **MapReduce Anatomy** describes the step-by-step lifecycle of how a MapReduce job is submitted, scheduled via YARN, executed in containers, and completed.

### ⬛ Mapper vs. Reducer Comparison (+ Helpers)
- **Combiner:** Mini-reducer running on the Mapper node to reduce network traffic.
- **Partitioner:** Routes intermediate keys to Reducers using `hash(key) % numReducers`.

| Feature | Mapper Phase | Reducer Phase |
|:--------|:-------------|:--------------|
| **Input** | Raw splits `<K1, V1>` | Sorted groups `<K2, List<V2>>` |
| **Output** | Intermediate `<K2, V2>` | Final aggregated `<K3, V3>` |
| **Storage** | Temporary **Local Disk** | Permanent **HDFS** |
| **Operation** | Filtering, parsing, mapping | Summation, counting, summarizing |

### ⬛ 6 Steps of MapReduce Job Anatomy
1. **Submission:** Client copies job JAR & splits to HDFS.
2. **Initialization:** ResourceManager launches **ApplicationMaster (AM)** in a Container.
3. **Assignment:** AM requests Containers for Map (Data Locality) & Reduce tasks.
4. **Execution:** NodeManagers download JAR from HDFS and run Map/Reduce tasks.
5. **Progress:** Tasks report progress every 3s to AM → Client.
6. **Completion:** Reducers write final output to HDFS and AM shuts down.

### ⬛ 2D Job Anatomy Diagram
```text
  [1. Client] --Submit--> [2. ResourceManager] --Launch--> [3. ApplicationMaster]
       |                                                        /          \
  (Copy JAR to HDFS) --> [ HDFS ] <--(Read/Write)-- [Map Container]  [Reduce Container]
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Data locality reduces network traffic; failed tasks automatically restart on another node.
- ❌ **Disadvantages:** High startup latency (creating containers/JVMs) makes it unsuitable for sub-second queries.

> 🟥 **Conclusion:** YARN's ApplicationMaster coordinates MapReduce tasks cleanly while maintaining fault tolerance and data locality.

---

## 📄 PAGE 16 — UNIT 3.1: INTRODUCTION TO NoSQL

### ⬛ Q. What is NoSQL? Explain its Characteristics and Applications. *(4/6 Marks)*
> 🟥 **Definition:** **NoSQL ("Not Only SQL")** refers to **non-relational, distributed databases** designed to store and query **unstructured, semi-structured, and massive datasets** without a fixed table schema.

### ⬛ Key Characteristics & Real-Life Applications
- **Schema-Free:** Store documents with different fields in the same collection (no `ALTER TABLE`).
- **Horizontal Scaling:** Easily scale out across hundreds of low-cost servers.
- **BASE Properties:** *Basically Available, Soft state, Eventual consistency* (prioritizes high speed & uptime).
- **Real-Life Applications:**
  1. **E-Commerce Catalogs:** Amazon/Flipkart products with varying attributes.
  2. **Social Media Feeds:** Instagram posts, likes, comments, and friend graphs.
  3. **IoT & Sensor Data:** Time-series temperature/GPS logs from smart devices.
  4. **Real-Time Caching & Gaming:** Fast user sessions and live leaderboards.

### ⬛ 2D Architecture Diagram
```text
  [ Mobile Apps ]   [ IoT Sensors ]   [ Social Media ]   [ E-Commerce ]
         \                 |                 |                 /
          v                v                 v                v
        +-------------------------------------------------------+
        |         NoSQL DATABASE (Schema-Free & Fast)           |
        |   [Document]    [Key-Value]    [Column]    [Graph]    |
        +-------------------------------------------------------+
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Handles mixed data formats, scales horizontally at low cost, ultra-fast read/write performance.
- ❌ **Disadvantages:** Lacks strict ACID transactions (eventual consistency) and standardized SQL query syntax.

> 🟥 **Conclusion:** NoSQL solves the speed, flexibility, and scaling bottlenecks of traditional relational databases.

---

## 📄 PAGE 17 — UNIT 3.2: TYPES OF NoSQL (DOCUMENT & KEY-VALUE)

### ⬛ Q. Explain Document-Based and Key-Value NoSQL Databases. *(4/6 Marks)*
> 🟥 **Definition:** **Document** and **Key-Value** databases are schema-less NoSQL stores optimized for flexible JSON objects and ultra-fast key lookups respectively.

### ⬛ 1. Document-Based Databases
- **How it works:** Stores data as semi-structured **JSON / BSON** documents inside collections. Each document can hold nested arrays and objects.
- **Examples:** **MongoDB**, CouchDB, Amazon DocumentDB.
- **Real Example:** Storing an e-commerce product or student profile (`{ "roll": 49, "name": "Amit", "skills": ["AI", "ML"] }`).

### ⬛ 2. Key-Value Stores
- **How it works:** Simplest NoSQL model storing data as unique **Key → Value** pairs (like a giant Python dictionary or hash table).
- **Examples:** **Redis**, Amazon DynamoDB, Riak.
- **Real Example:** Storing live user login sessions or shopping cart items (`"cart:49" -> "[Laptop, Mouse]"`).

### ⬛ 2D Structure Diagrams
```text
  DOCUMENT-BASED (MongoDB)               KEY-VALUE STORE (Redis)
  +-----------------------------+        +-------------+------------------+
  | {                           |        |     KEY     |      VALUE       |
  |   "roll_no": 49,            |        +-------------+------------------+
  |   "name": "Amit Kumar",     |        | "user:49"   | "Amit (Online)"  |
  |   "skills": ["AI", "ML"]    |        | "cart:49"   | "[Book, Pen]"    |
  | }                           |        +-------------+------------------+
  +-----------------------------+
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Blazing-fast lookups ($O(1)$ in Key-Value); zero schema-migration downtime in Document DBs.
- ❌ **Disadvantages:** Key-Value cannot query by value easily; Document DBs are weak at heavy multi-collection joins.

> 🟥 **Conclusion:** Choose **Document DBs** for rich app data and **Key-Value stores** for ultra-fast caching and sessions.

---

## 📄 PAGE 18 — UNIT 3.2: TYPES OF NoSQL (COLUMN & GRAPH)

### ⬛ Q. Explain Column-Oriented & Graph Databases + Compare All 4 Types. *(6 Marks)*
> 🟥 **Definition:** **Column-Oriented DBs** organize data by columns for massive analytical writes, while **Graph DBs** store entities as **Nodes** and relationships as **Edges**.

### ⬛ 3. Column-Oriented & 4. Graph-Based Databases
- **Column-Oriented:** Stores data in columns/column families instead of rows (**Apache Cassandra, HBase**). Best for IoT sensor logs & telecom billing.
- **Graph-Based:** Stores data as **Nodes** and **Edges** (**Neo4j, Amazon Neptune**). Best for social networks & fraud detection rings.

### ⬛ Master Comparison Table (4 Types of NoSQL)
| Type | Data Model | Examples | Best Real-World Use |
|:-----|:-----------|:---------|:--------------------|
| **1. Document** | JSON / BSON | MongoDB, CouchDB | Web apps, product catalogs |
| **2. Key-Value** | Key → Value | Redis, DynamoDB | Caching, shopping carts |
| **3. Column** | Column Families | Cassandra, HBase | IoT logs, time-series data |
| **4. Graph** | Nodes & Edges | Neo4j, Neptune | Social graphs, fraud rings |

### ⬛ 2D Diagrams (Column vs. Graph)
```text
  COLUMN-ORIENTED (Cassandra)             GRAPH-BASED (Neo4j)
  +--------+---------+--------+           ( Amit ) ---[STUDIES]---> ( AI & ML )
  | RowKey | Name    | Sem    |              | [FRIEND]
  +--------+---------+--------+              v
  |   49   | Amit    | 5th    |           ( Rahul )
  +--------+---------+--------+
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Column DBs handle huge write speeds; Graph DBs traverse deep friend/fraud links in milliseconds.
- ❌ **Disadvantages:** Graph DBs do not scale easily across many servers; Column DBs are harder to design for ad-hoc queries.

> 🟥 **Conclusion:** Selecting the right NoSQL type depends on whether your data is documents, pairs, logs, or connected graphs.

---

## 📄 PAGE 19 — UNIT 3.3 & 3.4: ADVANTAGES OF NoSQL & INDUSTRY USE

### ⬛ Q. Explain Advantages of NoSQL and Real-World Industry Case Studies. *(6 Marks)*
> 🟥 **Definition:** **Industry Adoption of NoSQL** demonstrates how global tech companies handle millions of concurrent users and petabytes of live data with zero downtime.

### ⬛ Unit 3.3 — Advantages & Disadvantages of NoSQL
| ✅ Advantages of NoSQL | ❌ Disadvantages of NoSQL |
|:-----------------------|:--------------------------|
| **Dynamic Schema:** Add new fields anytime without downtime. | **Eventual Consistency:** Trades strict ACID for higher speed. |
| **Elastic Horizontal Scaling:** Scale cheaply on commodity servers. | **No Standard Language:** Every DB has a different query API. |
| **High Throughput:** Fast read/write for real-time mobile/web apps. | **Limited Joins:** Complex multi-table joins are difficult. |

### ⬛ Unit 3.4 — Real-World Industry Case Studies
| Company | NoSQL Database | How They Use It in Real Life |
|:--------|:---------------|:-----------------------------|
| **Netflix** | **Apache Cassandra** | Tracks viewing history & playback position for crores of users globally. |
| **Amazon** | **DynamoDB** | Powers ultra-fast shopping carts & checkouts during Prime Day sales. |
| **Uber** | **Redis & Cassandra** | Tracks live driver GPS locations and matches riders in seconds. |
| **Facebook** | **HBase** | Stores billions of real-time Messenger messages and user feeds. |
| **LinkedIn** | **Neo4j / Espresso** | Maps 1st, 2nd, and 3rd-degree professional connections. |

### ⬛ 2D Industry Architecture Sketch
```text
  [Netflix: Cassandra] ---> Global Streaming History
  [Amazon: DynamoDB]   ---> High-Speed Shopping Carts
  [Uber: Redis]        ---> Live Driver GPS & Matching
```

> 🟥 **Conclusion:** Tech giants rely on NoSQL because traditional SQL cannot match its global scale and low-latency speed.

---

## 📄 PAGE 20 — UNIT 3.5, 3.6 & 3.7: SQL VS. NoSQL VS. NewSQL

### ⬛ Q. Compare SQL vs. NoSQL and Explain the Concept of NewSQL. *(6 Marks ★ Imp)*
> 🟥 **Definition:** **NewSQL** is a modern class of **relational databases** that combines the **ACID guarantees and SQL interface** of traditional RDBMS with the **horizontal scalability** of NoSQL.

### ⬛ Why NewSQL Was Needed & Examples
- SQL offers strong ACID safety for banking, but struggles to scale out globally. NoSQL scales horizontally, but sacrifices strict ACID transactions.
- **NewSQL** gives **both**: SQL + ACID + Horizontal Scaling! *Examples:* **Google Spanner, CockroachDB, VoltDB, TiDB**.

| Feature | SQL (MySQL/Oracle) | NoSQL (MongoDB/Redis) | NewSQL (Spanner/CockroachDB) |
|:--------|:-------------------|:----------------------|:-----------------------------|
| **Data Model** | Fixed Tables (Rows/Cols) | Document / KV / Column / Graph | **Fixed Relational Tables** |
| **Schema** | Static / Predefined | Dynamic / Schema-Free | **Static / Relational** |
| **Properties** | **ACID** | **BASE** (Eventual Consistency) | **ACID** |
| **Scaling** | Vertical (Scale-Up) | **Horizontal (Scale-Out)** | **Horizontal (Scale-Out)** |
| **Best Use Case** | College ERP, Accounting | Social Media, IoT, Caching | **Global Banking & FinTech** |

### ⬛ 2D Concept Diagram
```text
  [ Traditional SQL (ACID + Tables) ] + [ NoSQL (Horizontal Scale) ] ===> [ NewSQL ]
```

### ⬛ Advantages & Disadvantages of NewSQL
- ✅ **Advantages:** Familiar SQL queries, zero data-loss ACID safety, global horizontal scaling.
- ❌ **Disadvantages:** Higher memory/network overhead for distributed consensus (Paxos/Raft); still assumes structured tables.

> 🟥 **Conclusion:** NewSQL bridges SQL and NoSQL, making it ideal for mission-critical global financial applications.

---

## 📄 PAGE 21 — PRACTICAL: CREATING INDEXES FOR ENGINEERING DATA

### ⬛ Q. What is Indexing? Write Hands-On Commands for Engineering Data. *(4/6 Marks)*
> 🟥 **Definition:** An **Index** is a **special lookup data structure (usually B-Tree)** that speeds up database search queries from **$O(N)$ Full Scan** to **$O(\log N)$ Index Lookup**.

### ⬛ Hands-On Exercise: Indexing Machine Sensor Logs
Suppose an IoT engineering collection `machine_logs` stores:
`{ machine_id: "M-101", sensor: "Vibration", temp_c: 82.5, timestamp: ISODate("2026-11-26") }`

```javascript
// 1. MongoDB Single-Field Index (fast search by machine_id)
db.machine_logs.createIndex({ machine_id: 1 })

// 2. MongoDB Compound Index (filter machine + sort latest time)
db.machine_logs.createIndex({ machine_id: 1, timestamp: -1 })

// 3. Verify Speed using explain() -> Look for IXSCAN instead of COLLSCAN
db.machine_logs.find({ machine_id: "M-101" }).explain("executionStats")
```
```sql
-- Equivalent SQL Index
CREATE INDEX idx_machine_time ON machine_logs (machine_id, timestamp DESC);
```

### ⬛ 2D Performance Diagram
```text
  WITHOUT INDEX O(N):   [Row1]->[Row2]->[Row3]->...->[Row 10,00,000]  (Slow Scan!)
  WITH INDEX O(log N):  [B-Tree Index] ===(Direct Jump)===> [Target Row!] (Fast!)
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Cuts query time from seconds to milliseconds; improves sorting (`ORDER BY` / `.sort()`) speed.
- ❌ **Disadvantages:** Uses extra RAM/disk storage and slightly slows down `INSERT`/`UPDATE` writes.

> 🟥 **Conclusion:** Smart indexing on frequently queried fields is the fastest way to optimize engineering databases.

---

## 📄 PAGE 22 — PRACTICAL: EXPLORATORY DATA ANALYSIS (EDA) IN PYTHON

### ⬛ Q. What is EDA? Perform EDA on an Engineering Dataset in Python. *(6 Marks)*
> 🟥 **Definition:** **Exploratory Data Analysis (EDA)** is the process of **summarizing, cleaning, and visualizing datasets** in Python to uncover patterns, correlations, and anomalies before training ML models.

### ⬛ Sample Engineering Dataset (`machine_data.csv`) & Python Code
| Machine_ID | Temp_C | RPM | Vibration_mms | Status |
|:----------:|:------:|:---:|:-------------:|:------:|
| M1 | 65 | 1400 | 1.2 | Normal |
| M2 | 95 | 2300 | 5.1 | **Fault** |

```python
import pandas as pd
import matplotlib.pyplot as plt

df = pd.read_csv("machine_data.csv")
print(df.describe())                        # 1. Summary stats (mean, min, max)
print(df.isnull().sum())                    # 2. Check missing values
print(df[["Temp_C", "RPM", "Vibration_mms"]].corr())  # 3. Correlation matrix

# 4. Visualize Pattern (Scatter Plot)
plt.scatter(df["Temp_C"], df["Vibration_mms"], color="blue")
plt.title("Machine Temp vs Vibration")
plt.xlabel("Temperature (C)"); plt.ylabel("Vibration (mm/s)"); plt.show()
```
- 🟦 **Finding:** Machines with `Temp_C > 90°C` and `Vibration > 4.5 mm/s` strongly correlate with **Fault** status!

### ⬛ 2D Scatter Plot Diagram
```text
  Vibration ^      * (Fault: High Temp & Vibration)
    4.5+    |            *
    1.5     |   *   * (Normal)
            +-------------------> Temp (C)
                65   80   95
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Catches missing values/outliers early, improves ML model accuracy, reveals key features visually.
- ❌ **Disadvantages:** Time-consuming on messy Big Data; visual plots alone cannot handle 100+ features without dimensionality reduction.

> 🟥 **Conclusion:** EDA is a mandatory first step in Data Science to understand data quality and hidden trends before modeling.

---

## 📄 PAGE 23 — FUNCTIONAL DEPENDENCY & CLOSURE ($F^+$, $X^+$)

### ⬛ Q. Define Functional Dependency, Types & Closure ($F^+$ and $X^+$). *(6 Marks ★ Imp)*
> 🟥 **Definition:** A **Functional Dependency (FD)**, written **$X \rightarrow Y$**, means attribute(s) **$X$ (Determinant)** uniquely determine attribute(s) **$Y$ (Dependent)** in a relation $R$. *Ex:* `Roll_No -> Student_Name`.

### ⬛ Trivial vs. Non-Trivial Functional Dependency
| Type of FD | Condition | Explanation & Example |
|:-----------|:----------|:----------------------|
| **1. Trivial FD** | **$Y \subseteq X$** ($Y$ is subset of $X$) | Always true. *Ex:* `{Roll_No, Name} -> Name` |
| **2. Non-Trivial FD** | **$Y \not\subseteq X$** ($Y$ not subset of $X$) | Standard dependency. *Ex:* `Roll_No -> Course` |
| **3. Completely Non-Trivial** | **$X \cap Y = \emptyset$** (No common attr) | Disjoint sets. *Ex:* `Emp_ID -> Salary` |

### ⬛ Closure of FD Set ($F^+$) & Attribute Closure ($X^+$)
- 🟥 **$F^+$ (FD Closure):** Complete set of all FDs derived from $F$ using **Armstrong's Axioms**:
  1. **Reflexivity:** If $Y \subseteq X$, then $X \rightarrow Y$.
  2. **Augmentation:** If $X \rightarrow Y$, then $XZ \rightarrow YZ$.
  3. **Transitivity:** If $X \rightarrow Y$ and $Y \rightarrow Z$, then $X \rightarrow Z$.
- 🟥 **$X^+$ (Attribute Closure):** All attributes determined by $X$ (used to find **Candidate Keys**).
- 🟦 **Solved Example:** Given $R(A,B,C,D)$ and $F=\{A\rightarrow B,\; B\rightarrow C,\; C\rightarrow D\}$. Find **$A^+$**:
  - Start: $\{A\} \xrightarrow{A\rightarrow B} \{A,B\} \xrightarrow{B\rightarrow C} \{A,B,C\} \xrightarrow{C\rightarrow D} \{A,B,C,D\} = R \implies$ **$A$ is Candidate Key!**

### ⬛ 2D Diagram
```text
  TRIVIAL: {Roll, Name} -> Name   |   CLOSURE: {A} --(A->B)--> {A,B} --(B->C)--> {A,B,C} --(C->D)--> {A,B,C,D}
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Eliminates data redundancy (duplicates) and prevents insertion/update/deletion anomalies during normalization.
- ❌ **Disadvantages:** Over-normalizing tables using FDs creates many tables requiring slow SQL `JOIN`s.

> 🟥 **Conclusion:** Functional Dependency and Closure are the mathematical foundation for clean database normalization and Candidate Key discovery.

---

## 📄 PAGE 24 — UNIT 4.1: INTRODUCTION TO MONGODB & RDBMS COMPARISON

### ⬛ Q. What is MongoDB? Compare MongoDB with Traditional RDBMS. *(6 Marks)*
> 🟥 **Definition:** **MongoDB** is an **open-source, cross-platform, document-oriented NoSQL database** that stores data in flexible, JSON-like documents called **BSON** instead of fixed tables and rows.

### ⬛ Real-Life Example & RDBMS Comparison
- 🟦 **Real Example:** On Flipkart, a laptop has `{RAM, CPU, GPU}` while a shirt has `{Size, Color, Fabric}`. MongoDB stores both cleanly in one `products` collection without wasting empty columns!

| Feature | Traditional RDBMS (MySQL) | MongoDB (Document NoSQL) |
|:--------|:--------------------------|:-------------------------|
| **Data Structure** | Tables, Rows, Columns | **Collections, Documents, Fields** |
| **Schema** | Fixed / Static | **Dynamic / Flexible** |
| **Relationships** | Foreign Keys & `JOIN`s | **Embedded Docs** & References |
| **Scaling** | Vertical Scaling | **Horizontal Scaling (Sharding)** |
| **Query Language** | SQL (`SELECT`, `INSERT`) | **MQL** (`find()`, `insertOne()`) |

### ⬛ 2D Comparison Diagram
```text
  RDBMS (MySQL Table)                   MONGODB (Document)
  +----+--------+----------+            {
  | ID | Name   | Course   |              "roll_no": 49,
  +----+--------+----------+              "name": "Amit Kumar",
  | 49 | Amit   | AI & ML  |              "skills": ["AI", "Big Data"]
  +----+--------+----------+            }
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Schema flexibility, high read speed via embedded docs, easy horizontal sharding.
- ❌ **Disadvantages:** Max document size is **16 MB**; stores field names repeatedly (higher RAM usage).

> 🟥 **Conclusion:** MongoDB replaces rigid SQL tables with developer-friendly JSON/BSON documents for agile modern apps.

---

## 📄 PAGE 25 — UNIT 4.1 & 4.2: USE CASES, STORAGE MODEL & BSON

### ⬛ Q. Explain MongoDB Use Cases, Storage Hierarchy & BSON Format. *(6 Marks)*
> 🟥 **Definition:** **BSON (Binary JSON)** is the binary-encoded serialization format used internally by MongoDB to store documents efficiently and support rich data types.

### ⬛ Real-World Use Cases of MongoDB
1. **E-Commerce Catalogs:** Varying product attributes in one collection.
2. **IoT & Engineering Telemetry:** High-speed sensor readings from factory machines.
3. **CMS & Mobile Apps:** Blogs, user profiles, comments, and game leaderboards.

### ⬛ Data Storage Hierarchy & Why BSON?
- **Hierarchy:** **Database** (`college_db`) → **Collection** (like SQL Table) → **Document** (like SQL Row, max 16 MB) → **Field** (Key-Value pair).
- **Why BSON over plain JSON?** Faster machine parsing (binary length prefixes) + extra data types like **`ObjectId`** (unique 12-byte `_id`), **`Date`**, **`Int32/Int64`**, and **`Binary`**.

### ⬛ 2D Hierarchy Diagram
```text
  [MongoDB Server] --> [Database: eng_db] --> [Collection: machines] --> [BSON Doc: {_id, roll: 49}]
```

### ⬛ Advantages & Disadvantages of BSON
- ✅ **Advantages:** Faster traversal and type safety (`Date`, `Int32`) compared to text JSON.
- ❌ **Disadvantages:** Not directly human-readable without the MongoDB driver/shell converting it back to JSON.

> 🟥 **Conclusion:** MongoDB's Collection-Document hierarchy powered by BSON delivers both developer simplicity and high binary speed.

---

## 📄 PAGE 26 — UNIT 4.2: DATA MODELING & ENGINEERING SCHEMA DESIGN

### ⬛ Q. Compare Embedded vs. Referenced Data Model & Design an Engineering Schema. *(6 Marks)*
> 🟥 **Definition:** **Data Modeling in MongoDB** decides whether related data should be **Embedded** inside a single document or **Referenced** across separate collections via `_id`.

### ⬛ Embedded vs. Referenced Data Model
| Feature | Embedded Model (Denormalized) | Referenced Model (Normalized) |
|:--------|:------------------------------|:------------------------------|
| **Structure** | Sub-data nested inside **1 document** | Sub-data in a **separate collection** via `_id` |
| **Read Speed** | **Fastest** (1 single query) | Slower (2 queries or `$lookup`) |
| **Best For** | **1-to-1** or **1-to-Few** | **1-to-Many (Large)** or **Many-to-Many** |

### ⬛ Real Engineering Schema Design (Smart CNC Machine)
```json
// Collection 1: machines (Embed static specs — rarely changes)
{ "_id": "M-101", "name": "CNC Lathe", "specs": { "max_rpm": 3000, "kw": 15 } }

// Collection 2: sensor_logs (Reference via machine_id — grows every second!)
{ "_id": ObjectId("..."), "machine_id": "M-101", "temp_c": 74.2, "vibration": 1.8 }
```

### ⬛ 2D Schema Diagram
```text
  [ machines: _id="M-101" ] <---(References machine_id)--- [ sensor_logs: M-101, 74.2C ]
   (Embedded: specs)                                        (Unbounded Telemetry Logs)
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Hybrid design prevents hitting the 16 MB doc limit while keeping machine metadata instant to read.
- ❌ **Disadvantages:** Referenced data requires `$lookup` or application-level joins when combined reports are needed.

> 🟥 **Conclusion:** Good MongoDB schema design balances **Embedding** (for speed) with **Referencing** (for unbounded growth).

---

## 📄 PAGE 27 — UNIT 4.3: CRUD OPERATIONS (CREATE & READ)

### ⬛ Q. Explain Create and Read Operations in MongoDB Shell with Examples. *(4/6 Marks)*
> 🟥 **Definition:** **CRUD** stands for **Create, Read, Update, and Delete** — the four fundamental data manipulation operations executed in the **MongoDB Shell (`mongosh`)**.

### ⬛ 1. CREATE (Inserting Documents)
- **`insertOne()`** inserts 1 document; **`insertMany()`** inserts an array `[...]` of documents:
```javascript
db.students.insertOne({ roll_no: 49, name: "Amit Kumar", course: "AI & ML", sem: 5 })
db.students.insertMany([
  { roll_no: 50, name: "Rahul", sem: 5 },
  { roll_no: 51, name: "Priya", sem: 5 }
])
```

### ⬛ 2. READ (Retrieving Documents)
- **`find(query, projection)`** returns all matches; **`findOne()`** returns only the first match:
```javascript
db.students.find({ roll_no: 49 })                         // Exact match
db.students.find({ sem: { $gte: 5 } })                    // Filter: sem >= 5
db.students.find({}, { name: 1, _id: 0 })                 // Projection: show only name
db.students.findOne({ roll_no: 49 })                      // Single document
```

### ⬛ 2D CRUD Flow Diagram
```text
  [mongosh Shell] ---> insertOne/Many() ---> [MongoDB Collection] ---> find()/findOne() ---> [JSON Result]
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Clean JavaScript-like syntax; auto-generates unique `_id` if omitted; rich filter operators (`$gt`, `$in`).
- ❌ **Disadvantages:** Returning huge `find()` results without `.limit()` or projection can overload client memory.

> 🟥 **Conclusion:** `insertOne/Many` and `find/findOne` provide intuitive, JSON-native Create and Read capabilities in `mongosh`.

---

## 📄 PAGE 28 — UNIT 4.3: CRUD OPERATIONS (UPDATE & DELETE)

### ⬛ Q. Explain Update and Delete Operations in MongoDB Shell with Examples. *(4/6 Marks)*
> 🟥 **Definition:** **Update and Delete Operations** modify existing fields or remove unwanted documents from a MongoDB collection using atomic update operators like `$set` and `$inc`.

### ⬛ 3. UPDATE & 4. DELETE in MongoDB Shell (`mongosh`)
```javascript
// UPDATE: updateOne() & updateMany()
db.students.updateOne({ roll_no: 49 }, { $set: { sem: 6, city: "Barh" } })
db.students.updateMany({ course: "AI & ML" }, { $inc: { attendance: 1 } })

// DELETE: deleteOne() & deleteMany()
db.students.deleteOne({ roll_no: 51 })
db.students.deleteMany({ sem: 1 })
```

| CRUD | SQL Equivalent | MongoDB Shell (`mongosh`) |
|:-----|:---------------|:--------------------------|
| **Create** | `INSERT INTO` | `insertOne()` / `insertMany()` |
| **Read** | `SELECT` | `find()` / `findOne()` |
| **Update** | `UPDATE` | `updateOne()` / `updateMany()` |
| **Delete** | `DELETE` | `deleteOne()` / `deleteMany()` |

### ⬛ 2D Workflow Diagram
```text
  [Filter: {roll: 49}] ---> [Operator: $set / $inc] ---> [Document Updated Atomically!]
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Single-document updates are atomic; `$set` updates only specified fields without overwriting the whole document.
- ❌ **Disadvantages:** Running `deleteMany({})` with an empty filter deletes **every document** in the collection!

> 🟥 **Conclusion:** Mastering `updateOne/Many` and `deleteOne/Many` completes full data lifecycle management in MongoDB.

---

## 📄 PAGE 29 — UNIT 4.4: DATA MODELING BEST PRACTICES

### ⬛ Q. Explain Best Practices for Data Modeling in MongoDB. *(6 Marks)*
> 🟥 **Definition:** **MongoDB Data Modeling Best Practices** are design rules that maximize read/write speed, avoid the **16 MB document limit**, and align schema structure with application queries.

### ⬛ Top 6 Best Practices
1. **Design Around Query Patterns:** Model collections based on how your app reads and writes data most frequently.
2. **Embed 1-to-1 & 1-to-Few Data:** Keep tightly coupled objects (User + Address, Machine + Specs) together for 1-query reads.
3. **Reference 1-to-Many (Large) Data:** Never let arrays grow indefinitely inside a single document.
4. **Avoid Unbounded Arrays:** Store high-volume IoT logs in a separate collection referencing `machine_id`.
5. **Use Proper Data Types:** Store timestamps as `ISODate` (not strings) and numbers as `Int32/Double`.
6. **Bucket Pattern for Time-Series:** Group hourly sensor readings into 1 document per hour to cut document count.

### ⬛ 2D Decision Diagram
```text
  Is related data small & always read together?
        |
        +--- YES (1-to-1 / Few) ---> [ EMBED inside same Document ]
        +--- NO  (1-to-Many/Logs)--> [ REFERENCE in separate Collection ]
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Prevents 16 MB overflow errors, speeds up queries, lowers memory & disk I/O.
- ❌ **Disadvantages:** Denormalized (embedded) data can cause duplicate updates if shared fields change often.

> 🟥 **Conclusion:** Schema design in MongoDB should always follow your application's actual read/write access patterns.

---

## 📄 PAGE 30 — UNIT 4.4: INDEXING FOR PERFORMANCE OPTIMIZATION

### ⬛ Q. Explain Types of Indexes & Performance Optimization in MongoDB. *(6 Marks)*
> 🟥 **Definition:** **MongoDB Indexing** uses **B-Tree data structures** to turn slow full-collection scans (**`COLLSCAN`**) into fast index scans (**`IXSCAN`**). *(Every collection auto-indexes `_id`.)*

### ⬛ 5 Types of Indexes in MongoDB
| Index Type | Purpose & Syntax Example |
|:-----------|:-------------------------|
| **1. Single-Field** | Index on 1 field: `db.logs.createIndex({ machine_id: 1 })` |
| **2. Compound** | Index on 2+ fields: `db.logs.createIndex({ machine_id: 1, time: -1 })` |
| **3. Multikey** | Automatically indexes elements inside an **Array** field. |
| **4. Text Index** | Enables keyword search in strings: `{ notes: "text" }`. |
| **5. TTL Index** | Auto-deletes expired documents after $N$ seconds (great for temp logs!). |

### ⬛ 2D B-Tree Lookup Diagram
```text
  [Query: find({machine_id: "M-101"})]
         |
         +--> WITHOUT INDEX:  COLLSCAN (Checks every doc  -> Slow O(N))
         +--> WITH INDEX:     IXSCAN   (B-Tree direct jump -> Fast O(log N))
```

### ⬛ Advantages & Disadvantages
- ✅ **Advantages:** Drastically speeds up `find()`, `.sort()`, and range queries on millions of engineering records.
- ❌ **Disadvantages:** Consumes extra RAM and slightly slows down `insert`/`update` writes (indexes must also update).

> 🟥 **Conclusion:** Creating selective Single-Field, Compound, and TTL indexes optimizes MongoDB performance without wasting RAM.

---

*Subject: Big Data Analytics | AMIT KUMAR (AI & ML, 5th Sem, Roll No. 49) | Government Polytechnic Barh*
