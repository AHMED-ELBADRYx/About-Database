# الفهرس

- [الفهرس](#الفهرس)
  - [Databases](#databases)
    - [Basics - أساسيات](#basics---أساسيات)
      - [Database - قاعدة بيانات](#database---قاعدة-بيانات)
        - [Non-relational Database - قواعد البيانات الغير علائقية](#non-relational-database---قواعد-البيانات-الغير-علائقية)
          - [Types of Non-relational Databases - انواع قواعد البيانات الغير علائقية](#types-of-non-relational-databases---انواع-قواعد-البيانات-الغير-علائقية)
        - [Relational Database - قواعد البيانات العلائقية](#relational-database---قواعد-البيانات-العلائقية)
          - [Types of Relational Databases - انواع قواعد البيانات العلائقية](#types-of-relational-databases---انواع-قواعد-البيانات-العلائقية)
          - [Database Engines - محركات قواعد البيانات](#database-engines---محركات-قواعد-البيانات)
          - [SQL Software - برامج SQL](#sql-software---برامج-sql)
          - [Integrated Development Package - حزمة التطوير المتكاملة](#integrated-development-package---حزمة-التطوير-المتكاملة)
          - [Server](#server)
          - [Inquiries SQL - استعلامات SQL](#inquiries-sql---استعلامات-sql)
    - [SQL Server](#sql-server)
    - [MySQL](#mysql)
      - [Basic Queries - الاستعلامات الاساسية](#basic-queries---الاستعلامات-الاساسية)
      - [Date and Time - التاريخ والوقت](#date-and-time---التاريخ-والوقت)
      - [SQL Constraints - قيود SQL](#sql-constraints---قيود-sql)
        - [1. قيد `NOT NULL`](#1-قيد-not-null)
        - [2. قيد `UNIQUE`](#2-قيد-unique)
        - [3. قيد `CHECK`](#3-قيد-check)
        - [4. قيد `DEFAULT`](#4-قيد-default)
        - [5. قيد `PRIMARY KEY`](#5-قيد-primary-key)
          - [UNIQUE VS PRIMARY KEY](#unique-vs-primary-key)
        - [6. قيد `FOREIGN KEY`](#6-قيد-foreign-key)
          - [خيارات `ON DELETE` و `ON UPDATE`](#خيارات-on-delete-و-on-update)
        - [`AUTO_INCREMENT`](#auto_increment)
          - [`id SERIAL`](#id-serial)
        - [مثال كامل](#مثال-كامل)
      - [Relationships - العلاقات](#relationships---العلاقات)
        - [1. One to One Relation (علاقة واحد لواحد)](#1-one-to-one-relation-علاقة-واحد-لواحد)
        - [2. One to Many Relation (علاقة واحد لكثير)](#2-one-to-many-relation-علاقة-واحد-لكثير)
        - [3. Many to Many Relation (علاقة كثير لكثير)](#3-many-to-many-relation-علاقة-كثير-لكثير)
      - [JOINs - الوصلات](#joins---الوصلات)
        - [1. *INNER JOIN* - الربط الداخلي](#1-inner-join---الربط-الداخلي)
        - [2. *LEFT JOIN* - الربط الأيسر](#2-left-join---الربط-الأيسر)
        - [3. *RIGHT JOIN* - الربط الأيمن](#3-right-join---الربط-الأيمن)
        - [4. *FULL OUTER JOIN (UNION)* - الربط الخارجي الكامل](#4-full-outer-join-union---الربط-الخارجي-الكامل)
        - [5. *SELF JOIN* - الربط الذاتي](#5-self-join---الربط-الذاتي)
        - [6. *CROSS JOIN* - الربط التبادلي](#6-cross-join---الربط-التبادلي)
        - [أمثلة عملية مفصلة لكل نوع](#أمثلة-عملية-مفصلة-لكل-نوع)
      - [Advanced Select - الاختيار المتقدم](#advanced-select---الاختيار-المتقدم)
        - [Logical Operators - العمليات المنطقية](#logical-operators---العمليات-المنطقية)
        - [Calculations Operations - العمليات الحسابية](#calculations-operations---العمليات-الحسابية)
        - [Wildcards - أحرف البدل](#wildcards---أحرف-البدل)
        - [LIMITs - الحدود](#limits---الحدود)
        - [OFFSETs - الإزاحات](#offsets---الإزاحات)
        - [ORDER BY - الطلب حسب](#order-by---الطلب-حسب)
      - [Indexes - الفهارس](#indexes---الفهارس)
      - [Built-in Functions - الدوال المدمجة](#built-in-functions---الدوال-المدمجة)
        - [🔢 **الدوال الرياضية (Mathematical Functions)**](#-الدوال-الرياضية-mathematical-functions)
        - [📊 **دوال التجميع (Aggregate Functions)**](#-دوال-التجميع-aggregate-functions)
        - [📅 **دوال التاريخ والوقت (Date \& Time Functions)**](#-دوال-التاريخ-والوقت-date--time-functions)
        - [📝 **الدوال النصية (String Functions)**](#-الدوال-النصية-string-functions)
        - [🔍 **دوال الشرطية (Conditional Functions)**](#-دوال-الشرطية-conditional-functions)
        - [🛡️ **دوال الأمان (Security Functions)**](#️-دوال-الأمان-security-functions)
        - [📋 **الدوال الخاصة بـ JSON**](#-الدوال-الخاصة-بـ-json)
        - [🎯 **دوال التحقق من NULL**](#-دوال-التحقق-من-null)
        - [💾 **دوال لنظام وإدارة البيانات**](#-دوال-لنظام-وإدارة-البيانات)
        - [🚀 **أمثلة عملية للاستخدام في التطبيقات**](#-أمثلة-عملية-للاستخدام-في-التطبيقات)
      - [VIEW - العرض](#view---العرض)
      - [Prepared Statements - البيانات المعدة](#prepared-statements---البيانات-المعدة)
      - [Subquery - الاستعلام الفرعي](#subquery---الاستعلام-الفرعي)
      - [Stored Procedures - الإجراءات المخزنة](#stored-procedures---الإجراءات-المخزنة)
      - [Normalization - التطبيع](#normalization---التطبيع)
      - [Important MySQL Queries For Backend Developer](#important-mysql-queries-for-backend-developer)
        - [**استعلامات CRUD الأساسية**](#استعلامات-crud-الأساسية)
        - [**استعلامات التجميع والترتيب**](#استعلامات-التجميع-والترتيب)
        - [**JOINS - الربط بين الجداول**](#joins---الربط-بين-الجداول)
        - [**الاستعلامات المتقدمة**](#الاستعلامات-المتقدمة)
        - [**التعامل مع التواريخ والأوقات**](#التعامل-مع-التواريخ-والأوقات)
        - [**التعامل مع النصوص**](#التعامل-مع-النصوص)
        - [**التحكم في المعاملات (Transactions)**](#التحكم-في-المعاملات-transactions)
        - [**الإجراءات المخزنة والدوال**](#الإجراءات-المخزنة-والدوال)
        - [**التحسين والأداء**](#التحسين-والأداء)
        - [**الاستعلامات الأمنية**](#الاستعلامات-الأمنية)
        - [**استعلامات الصيانة**](#استعلامات-الصيانة)
        - [**استعلامات متقدمة للبيانات الكبيرة**](#استعلامات-متقدمة-للبيانات-الكبيرة)
    - [PostgreSQL](#postgresql)
      - [Summary - الملخص](#summary---الملخص)
        - [1. الأساسيات (`Must Know`)](#1-الأساسيات-must-know)
        - [2. تصميم قواعد البيانات](#2-تصميم-قواعد-البيانات)
        - [3. الاستعلامات المتقدمة](#3-الاستعلامات-المتقدمة)
        - [4. الأداء والتحسين](#4-الأداء-والتحسين)
        - [5. الميزات المتقدمة للمطورين](#5-الميزات-المتقدمة-للمطورين)
        - [6. الإدارة والأمان](#6-الإدارة-والأمان)
        - [7. التكامل مع لغات البرمجة](#7-التكامل-مع-لغات-البرمجة)
        - [8. أفضل الممارسات](#8-أفضل-الممارسات)
        - [9. مشروع عملي](#9-مشروع-عملي)
        - [10.  مصادر التعلم](#10--مصادر-التعلم)
      - [Detail - التفاصيل](#detail---التفاصيل)
        - [Phase 1: The Basics - المرحلة 1: الأساسيات](#phase-1-the-basics---المرحلة-1-الأساسيات)
          - [Basic Concepts and Installing - المفاهيم الأساسية والتثبيت](#basic-concepts-and-installing---المفاهيم-الأساسية-والتثبيت)
          - [Communication tools - أدوات الاتصال](#communication-tools---أدوات-الاتصال)
          - [Creating and Managing Databases - إنشاء وإدارة قواعد البيانات](#creating-and-managing-databases---إنشاء-وإدارة-قواعد-البيانات)
          - [Basic Operations (CRUD) - العمليات الأساسية](#basic-operations-crud---العمليات-الأساسية)
          - [Data Types and Constraints - أنواع البيانات والقيود](#data-types-and-constraints---أنواع-البيانات-والقيود)
        - [Phase 2: Advanced Queries - المرحلة 2: الاستعلامات المتقدمة](#phase-2-advanced-queries---المرحلة-2-الاستعلامات-المتقدمة)
          - [WHERE وترتيب النتائج](#where-وترتيب-النتائج)
          - [Built-in Functions - الدوال المـدمجة](#built-in-functions---الدوال-المـدمجة)
          - [Aggregations Functions - دوال التجميع](#aggregations-functions---دوال-التجميع)
          - [JOINS - الربط بين الجداول](#joins---الربط-بين-الجداول-1)
          - [Subqueries - الاستعلامات الفرعية](#subqueries---الاستعلامات-الفرعية)
          - [Window Functions - وظائف النافذة](#window-functions---وظائف-النافذة)
        - [Phase 3: Performance and Improvement - المرحلة 3: الأداء والتحسين](#phase-3-performance-and-improvement---المرحلة-3-الأداء-والتحسين)
          - [Indexes - الفهـارس](#indexes---الفهـارس)
          - [Query Performance Analysis - تحليل أداء الاستعلامات](#query-performance-analysis---تحليل-أداء-الاستعلامات)
          - [Advanced Optimization - التحسين المتقدم](#advanced-optimization---التحسين-المتقدم)
          - [Transactions - المعاملات](#transactions---المعاملات)
          - [Views](#views)
        - [Phase 4: Advanced Features - المرحلة 4: الميزات المتقدمة](#phase-4-advanced-features---المرحلة-4-الميزات-المتقدمة)
          - [Stored Procedures and Functions](#stored-procedures-and-functions)
          - [Triggers](#triggers)
          - [JSONB والبيانات شبه المنظمة](#jsonb-والبيانات-شبه-المنظمة)
          - [Full-Text Search](#full-text-search)
          - [Administration and Security - الإدارة والأمان](#administration-and-security---الإدارة-والأمان)
        - [Phase 5: Integration with Applications - المرحلة 5: التكامل مع التطبيقات](#phase-5-integration-with-applications---المرحلة-5-التكامل-مع-التطبيقات)
          - [التكامل مع Node.js](#التكامل-مع-nodejs)
          - [التكامل مع Python](#التكامل-مع-python)
          - [التكامل مع Java](#التكامل-مع-java)
          - [أفضل الممارسات والأمان](#أفضل-الممارسات-والأمان)
          - [مشروع نهائي متكامل](#مشروع-نهائي-متكامل)
        - [Final Exam - اختبار نهائي](#final-exam---اختبار-نهائي)
    - [The End - النهاية](#the-end---النهاية)

---

## Databases

---

### Basics - أساسيات

#### Database - قاعدة بيانات

- مجموعة جداول متراابطة من خلال `Key`

- `Tables`: الجداول
  - الجداول في قاعدة البيانات تتكون من مجموعة أعمدة أو حقول محددة تمثل خصائص الجدول وتتكون من صفوف أو سجلات تمثل البيانات التي تحمل قيم محددة لهذه الخصائص

- قواعد البيانات نوعان:
  - `Non-relational Database`: قواعد البيانات الغير علائقية
  - `Relational Database`: قواعد البيانات العلائقية

- `Multi-model Database`: قاعدة بيانات متعددة النماذج
  - تجمع بين النوعين لتكتسب فائدة كل نوع
  - أشهر محرك يتعامل معه: `fauna` ينشئ مفتاح يشير إلى قيمة تكون عبارة عن جداول مترابطة

##### Non-relational Database - قواعد البيانات الغير علائقية

- هي فئة عامة من قواعد البيانات المستقلة التي تشمل نماذج بيانات متنوعة مثل المستندات أو القيمة الرئيسية أو الرسوم البيانية أو الأعمدة العريضة وتستخدم مجموعة من التقنيات المختلفة المسماة `NoSQL` التي لا تستخدم `SQL` وتكون أكثر مرونة وقابلية للتوسع

- `NoSQL`: هي فئة واسعة من قواعد البيانات التي لا تتبع النوذج العلائقي التقليدي وهي لغة غير مترابطة تستخدم محركات مثل `mongoDB` عبارة عن أنماط تخزين تشبه الوثائق

###### Types of Non-relational Databases - انواع قواعد البيانات الغير علائقية

1. `Document-Based Database`: قاعدة بيانات مستندة إلى المستندات
   - مثل بيانات المريض فكل مريض له بيانات وحالات خاصة به
   - مثل مستندات `Json` التي تخزن بيانات `Json` بداخل بعض
   - مثل الطلبات التي تخزن بيانات الدفع وبيانات العنوان وبيانات التوصيل
   - أشهر محركات تتعامل مع هذا النوع: `mongoDB`,`Firebase`, `Cloud Firestore`

2. `Search-Based index Database`: قاعدة بيانات الفهرس القائمة على البحث
   - مكان يخزن توصيف البيانات لاستخدامها في عملية البحث فيحدد مكان البيانات في أي مستند
   - أشهر محركات تتعامل مع هذا النوع: `Elasticsaerch`, `Atlas Search` في `mongoDB` وهو يربط البحث ببيانات `mongoDB` للوصول إليها

3. `Key-Value Database`: قاعدة بيانات القيمة الرئيسية
   - يخزن البياناات على هيئة قاموس فينشئ مفتاح وقيمة له
   - له استخدامان:
     1. يمكن استخدامه كتخزين مؤقت (`Caching`) لبيانات تستخدم بكثرة ليتم الوصول إليها من خلال مفتاحها
     2. يمكن استخدامه كصف من هيكل بيانات يكون المفتاح فيه هو معرف البيانات والقيمة هي البيانات التي يتم تنفيذها
   - أشهر محرك يتعامل مع هذا النوع: `redis` (النسخة مفتوحة المصدر نسخة عالمية لشركة إيطالية والنسخة المدفوعة نسخة تجارية لشركة إسرائيلية)

4. `Wide-Column Database`: قاعدة بيانات ذات أعمدة عريضة
   - يخزن البيانات على هيئة قاموس مثل `Key-Value Database` لكن بدلا من أن تكون البيانات هي سلسلة بسيطة من القيم تكون عبارة عن أعمدة تخزن فيها القيم
   - يكون المفتاح مكان تخزين لأكثر من قيمة فيخزن البيانات بشكل مبسط وسريع
   - أشهر محركات تتعامل مع هذا النوع: `cassandra`, `DynamoDB` (تابع لأمازون)

##### Relational Database - قواعد البيانات العلائقية

- نوع معين من قواعد البيانات تخزن البيانات في جداول مهيكلة بصفوف وأعمدة وهي مثالية للبيانات المنظمة والعلاقات المعقدة وتستخدم لغة الاستعلامات الهيكلية (`SQL`)

- `Structured Query Language` (`SQL`): لغة استعلام منظمة مترابطة قياسية تستخدم للتفاعل مع قواعد البيانات العلائقية وتستخدم محركات مثل `MySQL` في إدارة وتحليل قواعد البيانات المترابطة `Relational Database`

- `Database Management System` (`DBMS`): نظام إدارة قواعد البيانات وهو سيرفر يتحكم بالنظام يتم استخدام `SQL` من خلاله ليتصل بالتطبيق والمستخدمين

###### Types of Relational Databases - انواع قواعد البيانات العلائقية

1. `Table-based schema`: مخطط قائم على الجدول يقوم بعمل علاقات على الجداول

   - أنواع العلاقات:
     - `OneToOne`: مثل علاقة الطالب من جدول الطلاب بدرجته من جدول الدرجات (درجة محددة لطالب محدد)
     - `OneToMany`: مثل علاقة الطالب من جدول الطلاب بدرجاته من جدول الدرجات (أكثر من درجة لطالب محدد)
     - `ManyToOne`: مثل علاقة الطلاب من جدول الطلاب بدرجتهم من جدول الدرجات (درجة محددة لأكثر من طالب)
     - `ManyToMany`: مثل علاقة الطلاب من جدول الطلاب بدرجاتهم من جدول الدرجات من خلال جدول ثالث يربط بينهما (أكثر من درجة لأكثر من طالب)
   - `Foreign key`: المفتاح الذي يقوم بالعلاقة ويتم وضعه بجدول `Many` في نوع `OneToMany` أو نوع `ManyToOne`أو نوع `ManyToMany` ويكون مفتاح لكل جدول بالجدول الثالث
   - أشهر محركات تتعامل مع هذا النوع: `PostgreSQL`, `MySQL`

2. `Graph Databases`: قواعد بيانات الرسوم البيانية ويستخدم بالعلاقات المعقدة بين البيانات وبدلا من أن تخزن في جداول يتم تخزينها في مدونة ملاحظات تحمل علاقات أكثر شمولية وتفصيلا
   - أشهر محرك يتعامل مع هذا النوع: `neo4j`

###### Database Engines - محركات قواعد البيانات

- `SQL Server`: خاص بمايكروسوفت

- `Oracle Database`: يتعامل مع كميات ضخمة من البيانات مناسب للشركات والمؤسسات الكبيرة

- `SQLite`: المعتمدة الرئيسية في الموبايل

- `PostgreSQL`: مدعومة بأغلب شركات الاستضافة

- `MySQL`: المعتمدة الرئيسية في الويب ومدعومة بأغلب شركات الاستضافة وبأغلب لغات البرمجة

###### SQL Software - برامج SQL

- `phpMyAdmin`: أداة إدارة لقواعد البيانات مدعومة بكل شركات الاستضافة تعمل مع `MySQL` أو `MariaDB` لها واجهة ويب لإدارة قواعد البيانات

- `HeidiSQL` (`HS`): يتعامل مع `MySQL` وغيرها من قواعد البيانات

###### Integrated Development Package - حزمة التطوير المتكاملة

- مثل `LARAGON` و `XAMPP` و `WAMP`
- تحتوي على خادم ويب (`Apache`/`Nginx`) و `PHP` و `MySQL` أو `MariaDB` وغيرها من الأدوات ويمكن تشغيل برامج `MySQL` مثل `phpMyAdmin` و `HeidiSQL` عليه

- التشبيه:
- `Laragon` ≈ مركز تجاري كامل يحتوي على بنك
- `MySQL`/`MariaDB` ≈ البنك
- `phpMyAdmin` ≈ برنامج لإدارة البنك

###### Server

- هي مفهوم عام في كل أنظمة قواعد البيانات وهو القلب الحقيقي للمحرك

- كل قاعدة بيانات تحتاج إلى خادم (`Database Server`) يقوم بـ:
  - استقبال طلبات المستخدمين (`Clients`)
  - تنفيذ أوامر `SQL`
  - إدارة الجداول والملفات والتخزين والاتصالات

--

- كل محرك قواعد بيانات مثل `MySQL` أو `PostgreSQL` أو `SQL Server` أو `Oracle` يحتوي على "خادم" خاص به يقوم بهذه الوظائف مثلاً:
  - `MySQL` → يستخدم `MySQL Server`
  - `PostgreSQL` → يستخدم `PostgreSQL Server`
  - `SQLite` → لا يستخدم أي خادم إطلاقًا (ملف واحد فقط)
  - `Microsoft SQL Server` → يستخدم خادم خاص بمايكروسوفت

- مثال للتوضيح:
  - عندما تثبت `MySQL`، أنت تثبت:
    - `MySQL Server` ← الخادم الذي يشغل قاعدة البيانات.
    - `MySQL Workbench` ← أداة رسومية للتعامل مع الخادم.
  
  - عندما تثبت `Microsoft SQL Server`، أنت تثبت:
    - `SQL Server Engine` ← خادم مايكروسوفت.
    - `SQL Server Management Studio` (`SSMS`) ← الأداة الرسومية.

- القاعدة العامة:
  - أغلب محركات `SQL` تعتمد على وجود شيئين رئيسيين:
  1️⃣ خادم يشغل قاعدة البيانات (`Server Engine`)
  2️⃣ أداة رسومية أو واجهة لإدارة الخادم (`Client` / `GUI Tool`)
    - تسهل التعامل مع الخادم بدلًا من كتابة الأوامر يدويًا مثلاً:
      - `MySQL` → أداة اسمها `Workbench`
      - `PostgreSQL` → أداة اسمها `pgAdmin`
      - `SQL Server` → أداة اسمها `SSMS` (`SQL Server Management Studio`)
      - `HeidiSQL` → أداة اسمها `Laragon`
      - `phpMyAdmin` → أداة اسمها `XAMPP`
    - لكنها ليست ضرورية دائمًا — يمكنك التعامل مع الخادم من سطر الأوامر (`CLI`) فقط إن أردت.

- الاستثناءات (التي لا تحتاج خادم)
  
  - ليست كل محركات `SQL` تحتاج `Server`. أشهر استثناء هو:
    - `SQLite`: لا يوجد خادم إطلاقًا فكل قاعدة بيانات هي ملف واحد فقط (`.db` أو `.sqlite`).

  - البرنامج الذي يستخدمها مثل `Python` أو `Android` يتصل مباشرة بالملف. هذا يجعلها خفيفة جدًا وسهلة الاستخدام في التطبيقات الصغيرة.

--

###### Inquiries SQL - استعلامات SQL

- `CREATE`: إنشاء قاعدة البيانات
- `INSERT`: إدخال البيانات في قاعدة البيانات
- `UPDATE`: تعديل البيانات
- `DELETE`: حذف البيانات
- `RETRIEVE`: التعامل مع البيانات والتحكم في عرضها

---

### SQL Server

- يتم تنزيل المحرك من خلال البحث على [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads) واختيار `SQL Server 2022 Developer` للتنزيل
- بيئة العمل المطلوب تنزيلها هي [SQL Server Management Studio (SSMS)](https://learn.microsoft.com/en-us/ssms/install/install)

- *الكلمات المفتاحية يمكن كتابتها بأحرف صغيرة أو كبيرة*
- *لا يلزم وضع ; بنهاية السطر*

---

### MySQL

- تنزيل `MySQL`:
  - البحث عنه في جوجل أو من [هنا](https://dev.mysql.com/downloads/windows/installer/8.0.html) مباشرة
  - اختر `Costom` ثم أضف `Server` و `Workbench` للتنزيل
  - الشرح الحالى خاص بالإصدار `8`

- تنزيل `Databases`:
- يمكن تنزيل قاعدة بيانات جاهزة من خلال [MySQL Sample Database](https://www.mysqltutorial.org/getting-started-with-mysql/mysql-sample-database/)
- بعد عملية التنزيل يمكن نسخ نص الملف ولصقه في `Workbench` لإضافته

- *الكلمات المفتاحية يمكن كتابتها بأحرف صغيرة أو كبيرة*
- *يتم وضع ; بنهاية السطر لإضافة سطر جديد*

--

#### Basic Queries - الاستعلامات الاساسية

- أنشاء تعليق غير قابل للتنفيذ:

```sql
-- This is a comment
```

- معرفة رقم الإصدار:

```SQL
SELECT VERSION();
-- 8.0.43
```

- `CREATE`: إنشاء قاعدة بيانات

```sql
CREATE DATABASE db_name;
```

- `USE`: تحديد قاعدة البيانات التي يتم تنفيذ الاستعلامات عليها

```sql
USE db_name;
```

- `DROP`: حذف قاعدة بيانات

```sql
DROP DATABASE db_name;
```

- `ALTER`: تعديل القاعدة
  - يمكن تنفيذ أكثر من تعديل
  - `READ ONLY = 1`: تفعيل القراءة فقط
  - `READ ONLY = 0`: إلغاء تفعيل القراءة فقط
  - `COLLATE`: للتعامل مع اللغة

```sql
ALTER DATABASE db_name READ ONLY = 1;
ALTER DATABASE db_name READ ONLY = 0 DEFAULT COLLATE utf8mb4_bin;
```

- `CREATE`: أنشاء جدول:
  - داخلهيتم إنشاء الحقول ونوع بياناتها وعدد الرموز داخلها مثل:
    - `INT`: القيمة الرقمية
    - `VARCHAR`: القيمة النصية (يجب تحديد الطول)

```sql
CREATE TABLE table_name(
  column_id INT,
  column_name VARCHAR(50),
  column_mark DECIMAL(5, 2) -- (maximum place integer and decimal, maximum place decimal)
);
```

- `RENAME`: تغيير اسم الجدول

```sql
RENAME TABLE table_name TO table_updated_name;
```

- `SHOW`: عرض جداول القاعدة:

```sql
SHOW TABLES;
```

- `ALTER`: تعديل الجدول
  - `ADD`: إضافة عمود
  - `RENAME`: تغيير اسم العمود (في MySQL 8.0+)
  - `MODIFY`: تغيير نوع البيانات والموقع
    - `AFTER`: وضع العمود بعد عمود معين
    - `FIRST`: وضع العمود بالبداية
  - `CHANGE`: تغيير الاسم والنوع والموقع
  - `DROP`: حذف العمود

```sql
-- إضافة العمود
ALTER TABLE table_name 
ADD COLUMN new_column VARCHAR(10);

-- إعادة تسمية العمود
ALTER TABLE table_name
RENAME COLUMN new_column TO updated_column;

-- تغيير نوع البيانات ونقله
ALTER TABLE table_name
MODIFY COLUMN updated_column INT AFTER column_name;

-- ALTER TABLE table_name 
-- MODIFY COLUMN updated_column INT FIRST;

-- تغيير الاسم
-- ALTER TABLE table_name 
-- CHANGE COLUMN old_name new_name VARCHAR(10);
-- يجب تكرار نوع البيانات الأصلي

-- تغيير النوع
-- ALTER TABLE table_name 
-- CHANGE COLUMN column_name column_name INT;
-- تكرار نفس اسم العمود مع نوع جديد

-- تغيير الموقع
-- ALTER TABLE table_name 
-- CHANGE COLUMN column_name column_name VARCHAR(10) AFTER other_column;
-- تكرار نفس الاسم والنوع مع تحديد موقع جديد

-- تعديل العمود (تغيير الاسم والنوع والموقع)
-- ALTER TABLE table_name
-- CHANGE COLUMN new_column updated_column INT AFTER column_name;

-- حذف العمود
ALTER TABLE table_name
DROP COLUMN updated_column;
```

- حذف الجدول

```sql
DROP TABLE table_name

-- الحصول على قائمة بجميع الجداول
SHOW TABLES;

-- ثم حذف كل جدول
DROP TABLE table1, table2, table3, ...;

-- حذف الجدول إن كان موجودا
DROP TABLE IF EXISTS table_name
```

- `INSERT`: إدخال بيانات
  - يمكن إدخال أكثر من صف من البيانات
  - يمكن تحديد حقل معين فقط تضاف إليه البيانات

```sql
INSERT INTO table_name VALUES (1, "Value name 1", 150.25);
INSERT INTO table_name VALUES
(2, "Value name 2", 10.5),
(3, "Value name 3", 7.03),
(4, "Value name 4", 80.5);
INSERT INTO table_name (column_id, column_name) VALUES (5, "Value name 5");
```

- `SHOW`: عرض أعمدة الجدول:

```sql
SHOW COLUMNS FROM table_name;
```

- `SELECT`: عرض بيانات الجدول
  - `*`: كل الأعمدة
  - يمكن عرض أعمدة معينة بترتيب معين (غير مؤثر على الترتيب الأصلي)
  - `WHERE`: تحديد صف أو صفوف معينة

```sql
SELECT * FROM table_name;
SELECT column_name, column_id FROM table_name;
SELECT * FROM table_name WHERE column_id = 1;
SELECT * FROM table_name WHERE column_name = "Value name 2";
SELECT * FROM table_name WHERE column_id >= 3;
SELECT * FROM table_name WHERE column_id != 5; -- !=: لا تساوي
SELECT * FROM table_name WHERE column_mark IS NULL; -- IS NULL: بلا قيمة
SELECT * FROM table_name WHERE column_mark IS NOT NULL;
```

- `UPDATE`: تعديل البيانات

```sql
UPDATE table_name SET column_mark = 50 WHERE column_id = 5;
UPDATE table_name SET column_name = "Value name 20", column_mark = 30.5 WHERE column_id = 2;

UPDATE table_name
SET column_mark = 100 
WHERE primary_key_column IN (SELECT primary_key_column FROM table_name); -- يتم تعديلها على كل الصفوف
-- primary_key_column: اسم العمود الرئيسي المضاف إليه Primary Key
```

- `DELETE`: حذف البيانات

```sql
DELETE FROM table_name WHERE column_id = 5;

-- حذف كل الصفوف
DELETE FROM table_name
WHERE primary_key_column IN (SELECT primary_key_column FROM table_name);

-- أو الأفضل من استخدام IN مع subquery
DELETE FROM table_name 
WHERE primary_key_column IS NOT NULL;

-- أو الأسرع TRUNCATE: يحذف الجدول كاملاً ويعيد إنشائه، لا يقبل WHERE
TRUNCATE TABLE table_name;
```

--

#### Date and Time - التاريخ والوقت

- أنواع بيانات التاريخ والوقت:
  - `DATE`:  التاريخ
  - `TIME`: الوقت
  - `DATETIME`: التاريخ والوقت

```sql
CREATE TABLE table_time(
  column_date DATE,
  column_time TIME,
  column_datetime DATETIME
);
```

- بيانات الإدخال للتاريخ والوقت الحالي:
  - `CURRENT_DATE()`: التاريخ الحالي لنوع `DATE`
  - `CURRENT_TIME()`: الوقت الحالي لنوع `TIME`
  - `NOW()`: التاريخ والوقت الحالي لنوع `DATETIME`

```sql
INSERT INTO table_time VALUES (CURRENT_DATE(), CURRENT_TIME(), NOW());
```

--

#### SQL Constraints - قيود SQL

- `NOT NULL`: يجعل قيمة العمود غير فارغة

- `UNIQUE`: يفرض فقط أن القيم فريدة، لكنه لا يفرض `NOT NULL` بشكل افتراضي، لذا عادةً يمكن أن يحتوي العمود على قيم `NULL` (وسلوك التعامل مع `NULL` قد يسمح بعدد من الـ `NULLs` حسب نظام قاعدة البيانات — لكن أغلب المحركات تعتبر `NULL` غير متساوية وتسمح بعدة `NULLs`).

- `PRIMARY KEY`: يفرض أن القيم فريدة (`unique`) وغير فارغة (`NOT NULL`)، ويُستخدم لتعريف المفتاح الأساسي الذي يميِّز كل صف في الجدول. كما أن لكل جدول مفتاح أساسي واحد فقط.

- `CHECK`: يجعل بيانات العمود لها شرط معين

- `DEFAULT`: القيمة الافتراضية إذا لم تضاف أي قيمة

- `FOREIGN KEY`: يربط عمود الجدول بعمود جدول آخر يشترك معه بنفس نوع البيانات

--

- العثور على أسماء القيود:

```sql
SELECT CONSTRAINT_NAME 
FROM INFORMATION_SCHEMA.TABLE_CONSTRAINTS 
WHERE TABLE_NAME = 'table_name';
```

--

##### 1. قيد `NOT NULL`

*الوظيفة*: يمنع الحقل من قبول القيم الفارغة (`NULL`)

```sql
-- الإضافة أثناء إنشاء الجدول:
CREATE TABLE employees(
    employee_id INT,
    employee_name VARCHAR(255) NOT NULL
);

-- الإضافة بعد إنشاء الجدول:
ALTER TABLE employees
MODIFY employee_name VARCHAR(255) NOT NULL;

-- هذا سيعمل:
INSERT INTO employees VALUES(1, 'أحمد');

-- هذا سيفشل لأن employee_name لا يمكن أن يكون NULL:
INSERT INTO employees VALUES(2, NULL);

-- الإزالة بعد الإضافة
ALTER TABLE employees
MODIFY employee_name VARCHAR(255) NULL;
```

##### 2. قيد `UNIQUE`

*الوظيفة*: يضمن أن جميع القيم في الحقل مختلفة

```sql
-- الإضافة أثناء إنشاء الجدول:
CREATE TABLE products(
    product_id INT UNIQUE,
    product_name VARCHAR(255)
);

-- الإضافة بعد إنشاء الجدول:
ALTER TABLE products 
ADD UNIQUE (product_id);

-- أو مع اسم للقيد
ALTER TABLE products 
ADD CONSTRAINT unique_product_id UNIQUE (product_id);

-- هذا سيعمل:
INSERT INTO products VALUES(1, 'منتج 1');
INSERT INTO products VALUES(2, 'منتج 2');

-- هذا سيفشل لأن product_id مكرر:
INSERT INTO products VALUES(1, 'منتج 3');

-- الإضافة على عدة أعمدة:
ALTER TABLE products
ADD CONSTRAINT unique_id_name UNIQUE (product_id, product_name);

-- هذا سيعمل:
INSERT INTO products VALUES(3, 'منتج 2');

-- هذا سيفشل لأن unique_id_name مكرر:
INSERT INTO products VALUES(3, 'منتج 1');

-- الإزالة بعد الإضافة:
ALTER TABLE products
DROP INDEX unique_product_id;
```

##### 3. قيد `CHECK`

*الوظيفة*: يتحقق من أن القيم تحقق شرطاً معيناً

```sql
-- الإضافة أثناء إنشاء الجدول:
CREATE TABLE students(
    student_id INT,
    student_age INT CHECK (student_age >= 18),
    grade VARCHAR(1) CHECK (grade IN ('A', 'B', 'C', 'D', 'F'))
);

-- الإضافة بعد إنشاء الجدول:
ALTER TABLE students
ADD CONSTRAINT age_check CHECK (student_age >= 18);

-- هذا سيعمل:
INSERT INTO students VALUES(1, 20, 'A');

-- هذا سيفشل لأن العمر أقل من 18:
INSERT INTO students VALUES(2, 16, 'B');

-- هذا سيفشل لأن الدرجة غير مسموحة:
INSERT INTO students VALUES(3, 19, 'E');

-- الإزالة بعد الإضافة:
ALTER TABLE students DROP CONSTRAINT age_check;
```

##### 4. قيد `DEFAULT`

*الوظيفة*: يعطي قيمة افتراضية للحقل إذا لم يتم إدخال قيمة

```sql
-- الإضافة أثناء إنشاء الجدول:
CREATE TABLE orders(
    order_id INT,
    order_date DATE DEFAULT (CURRENT_DATE()),
    order_status VARCHAR(20) DEFAULT 'معلق'
);

-- الإضافة بعد إنشاء الجدول:
ALTER TABLE orders
ALTER order_status SET DEFAULT 'معلق';

-- سيستخدم القيم الافتراضية:
INSERT INTO orders (order_id) VALUES(1);

-- النتيجة: (1, '2024-01-01', 'معلق') - إذا كان تاريخ اليوم 2024-01-01

-- الإزالة بعد الإضافة:
ALTER TABLE orders ALTER order_status DROP DEFAULT;
```

##### 5. قيد `PRIMARY KEY`

*الوظيفة*: يجمع بين `NOT NULL` و `UNIQUE` ويعرف المفتاح الرئيسي

```sql
-- الإضافة أثناء إنشاء الجدول:
CREATE TABLE customers(
    customer_id INT PRIMARY KEY,
    customer_name VARCHAR(255)
);

-- الإضافة بعد إنشاء الجدول:
ALTER TABLE customers
ADD CONSTRAINT customer_pk PRIMARY KEY (customer_id);

INSERT INTO customers VALUES
(1, "عميل 1"), -- هذا سيعمل
(1, "عميل 2"), -- هذا سيفشل لأن customer_id مكرر
(NULL, "عميل 3"); -- هذا سيفشل لأن لا يمكن أن يكون NULL

-- الإزالة بعد الإضافة:
ALTER TABLE customers DROP PRIMARY KEY;
```

--

###### UNIQUE VS PRIMARY KEY

- يمكنك تعريف عدة قيود `UNIQUE` في جدول واحد، لكن `PRIMARY KEY` مفتاحًا أساسيًا واحدًا فقط مسموحًا به لكل جدول.

- `PRIMARY KEY` غالبًا ما يُنشئ فهرسًا (`index`) خاصًا — وفي بعض المحركات (مثل `InnoDB` في `MySQL`) يكون مفهرسًا مكدَّسًا (`clustered index`)، بينما `UNIQUE` يُنشئ فهرسًا فريدًا غير مكدَّس عادة.

- السلوك مع `NULL`: معظم قواعد البيانات تعتبِر `NULL` قيمة غير محددة وبالتالي تسمح بعدة صفوف فيها `NULL` لعمود به قيد `UNIQUE`، بينما `PRIMARY KEY` لا يسمح بـ `NULL` أبداً.

- مثال عملي: عمود `email UNIQUE` يمكن أن يقبل أكثر من صف بقيمة `NULL` في كثير من أنظمة `DB`.

- يمكنك تحقيق سلوك `"unique + not null"` عبر:
  - تعريف `PRIMARY KEY`
  - تعريف `UNIQUE + NOT NULL` معًا (لكن تبقى فرق إدارية: ليس مفتاحًا أساسيًا رسميًا).

أمثلة:

- `PRIMARY KEY` (`UNIQUE` + `NOT NULL`)

```sql
CREATE TABLE users (
  id INT PRIMARY KEY,   -- فريد وغير فارغ، ومفتاح أساسي
  username TEXT NOT NULL
);
```

- `UNIQUE` يسمح بـ `NULL` في معظم الأنظمة

```sql
CREATE TABLE people (
  id SERIAL PRIMARY KEY,
  email VARCHAR(255) UNIQUE  -- يمكن أن يقبل NULLs في كثير من أنظمة DB
);

INSERT INTO people (email) VALUES (NULL), (NULL); -- غالبًا مسموح
```

- جعل `UNIQUE` + `NOT NULL` (مكافئ عمليًا لكنه ليس `"PRIMARY"`)

```sql
CREATE TABLE items (
code VARCHAR(50) NOT NULL UNIQUE
);
```

--

*عدد قيود `PRIMARY KEY` و `UNIQUE` المضافة في الجدول*

--

🎯 أولًا: `PRIMARY KEY`

- كل جدول يمكن أن يحتوي على مفتاح أساسي واحد فقط.
- هذا المفتاح يمكن أن يكون:
  - عمودًا واحدًا (`Single Column Key`)
  - عدة أعمدة معًا (`Composite Primary Key`).
  - لكنه لا يمكن أن يكون أكثر من مفتاح أساسي واحد في الجدول.

- مثال 1: مفتاح أساسي لحقل واحد:

```sql
CREATE TABLE users (
    id INTEGER PRIMARY KEY,
    username TEXT
);
```

- مثال 2: مفتاح أساسي مركّب من أكثر من حقل:

```sql
CREATE TABLE orders (
    id INTEGER,
    product_id INTEGER,
    PRIMARY KEY (id, product_id)
);
```

> هنا لا يوجد مفتاح أساسي آخر، لكن المفتاح الأساسي مكوّن من حقلين معًا، ويجب أن يكون كل ثنائي (`id` + `product_id`) فريدًا.

--

🔑 ثانيًا: `UNIQUE`

- يمكنك إضافة عدة قيود `UNIQUE` في نفس الجدول.
- ويمكن أن تكون:
  - على عمود واحد.
  - أو على عدة أعمدة معًا (لتكوين فريدة مشتركة).

- مثال 1: عدة قيود فريدة:

```sql
CREATE TABLE employees (
    id INTEGER PRIMARY KEY,
    email TEXT UNIQUE,
    phone TEXT UNIQUE
);
```

> هنا يوجد مفتاح أساسي واحد فقط (`id`)،
لكن هناك قيود فريدة إضافية (`email` و `phone`).

- مثال 2: قيد فريد مركّب:

```sql
CREATE TABLE reservations (
    room_id INTEGER,
    res_date DATE,
    UNIQUE (room_id, res_date)
);
```

> هذا يمنع وجود أكثر من حجز لنفس الغرفة في نفس التاريخ،
لكنه لا يمنع تكرار الغرفة في تواريخ مختلفة (ولا يعتبر مفتاحًا أساسيًا رسميًا).

--

دائمًا استخدم `PRIMARY KEY` لتحديد السجل بشكل واضح (غالبًا id).

استخدم `UNIQUE` عندما تريد ضمان عدم تكرار قيمة معينة (مثل `email` أو `username`).

وإذا احتجت منع تكرار تركيبة محددة من القيم (مثل `room_id` + `date`) استخدم `UNIQUE` المركّب.

--

##### 6. قيد `FOREIGN KEY`

*الوظيفة*: يربط عمود الجدول بعمود جدول آخر يشترك معه بنفس نوع البيانات

```sql
-- الإضافة أثناء إنشاء الجدول
CREATE TABLE departments(
    dept_id INT PRIMARY KEY,
    dept_name VARCHAR(100)
);

CREATE TABLE employees(
    emp_id INT PRIMARY KEY,
    emp_name VARCHAR(100),
    dept_id INT,
    FOREIGN KEY (dept_id) REFERENCES departments(dept_id)
);

-- تحديد اسم المفتاح
CREATE TABLE employees (
    emp_id INT PRIMARY KEY,
    emp_name VARCHAR(50),
    dept_id INT,
    CONSTRAINT fk_emp_dept 
        FOREIGN KEY (dept_id) REFERENCES departments(dept_id)
);

-- الإضافة بعد إنشاء الجدول
ALTER TABLE employees
ADD CONSTRAINT fk_emp_dept
FOREIGN KEY (dept_id) 
REFERENCES departments(dept_id);

-- معرفة اسم CONSTRAINT
SHOW CREATE TABLE employees;
-- أو
SELECT CONSTRAINT_NAME 
FROM information_schema.KEY_COLUMN_USAGE
WHERE TABLE_NAME = 'employees' 
AND REFERENCED_TABLE_NAME IS NOT NULL;

-- الإزالة بعد الإضافة:
ALTER TABLE employees DROP FOREIGN KEY fk_emp_dept;
```

--

###### خيارات `ON DELETE` و `ON UPDATE`

1. *CASCADE* (التسلسل)

    ```sql
    FOREIGN KEY (dept_id) REFERENCES departments(dept_id)
    ON DELETE CASCADE
    ON UPDATE CASCADE;
    -- عند حذف قسم، تحذف جميع موظفيه تلقائياً
    ```

2. *SET NULL* (تعيين NULL)

    ```sql
    FOREIGN KEY (dept_id) REFERENCES departments(dept_id)
    ON DELETE SET NULL;
    -- عند حذف قسم، يصبح dept_id = NULL للموظفين
    ```

3. *RESTRICT* أو *NO ACTION* (المنع)

    ```sql
    FOREIGN KEY (dept_id) REFERENCES departments(dept_id)
    ON DELETE RESTRICT;
    -- يمنع حذف القسم إذا كان لديه موظفين (الخيار الافتراضي)
    ```

4. *SET DEFAULT* (تعيين القيمة الافتراضية)

    ```sql
    FOREIGN KEY (dept_id) REFERENCES departments(dept_id)
    ON DELETE SET DEFAULT;
    -- يعين القيمة الافتراضية لـ dept_id
    ```

--

- فوائد ومميزات `FOREIGN KEY`

1. *سلامة البيانات (Data Integrity)*

    ```sql
    -- يمنع إدخال قيم غير موجودة في الجدول المرجعي
    INSERT INTO orders (id, product_id) 
    VALUES (999, 1); -- ❌ فشل إذا id 999 غير موجود
    ```

2. *التماسك المرجعي (Referential Integrity)*

    ```sql
    -- يمنع حذف سجلات يتم الرجوع إليها
    DELETE FROM users WHERE id = 1; 
    -- ❌ فشل إذا كان هناك طلبات مرتبطة بهذا المستخدم
    ```

3. *توثيق العلاقات*

   - يوضح العلاقات بين الجداول بشكل واضح
   - يساعد في فهم هيكل قاعدة البيانات

4. *الاستعلامات المرتبطة*

    ```sql
    -- استعلامات JOIN أكثر كفاءة
    SELECT e.emp_name, d.dept_name
    FROM employees e
    JOIN departments d ON e.dept_id = d.dept_id;
    
    -- بنفس الكفاءة
    SELECT e.emp_name, d.dept_name
    FROM employees e
    INNER JOIN departments d ON e.dept_id = d.dept_id;
    ```

- معنى واستخدامات استعلامات `JOIN`

- *الوظيفة الأساسية:*
  - *ربط بيانات من جدولين مختلفين معاً في نتيجة واحدة*

*مثال عملي:*

- الجداول الموجودة:

*جدول الموظفين (employees):*

| emp_id | emp_name | dept_id |
|--------|----------|---------|
| 1      | أحمد     | 101     |
| 2      | محمد     | 102     |
| 3      | خالد     | 101     |

*جدول الأقسام (departments):*

| dept_id | dept_name |
|---------|-----------|
| 101     | المبيعات  |
| 102     | التقنية   |

*نتيجة الاستعلام:*

```sql
SELECT e.emp_name, d.dept_name
FROM employees e
JOIN departments d ON e.dept_id = d.dept_id;
```

*ستعطي:*

| emp_name | dept_name |
|----------|-----------|
| أحمد     | المبيعات  |
| محمد     | التقنية   |
| خالد     | المبيعات  |

*بدون `JOIN` سنحصل على هذه النتيجة من خلال سنحتاج استعلامين منفصلين ثم دمج النتائج يدوياً!*

--

- مميزات وعيوب `FOREIGN KEY`

*المميزات:*

- ✓ الحفاظ على سلامة البيانات
- ✓ منع البيانات اليتيمة (Orphaned Records)
- ✓ تحسين أداء الاستعلامات المرتبطة
- ✓ توثيق العلاقات بين الجداول

*العيوب:*

- ✗ تعقيد في عمليات الحذف والتحديث
- ✗ قد تؤثر على الأداء في الجداول الكبيرة جداً
- ✗ صعوبة في استيراد البيانات بترتيب خاطئ

--

##### `AUTO_INCREMENT`

- *زيادة رقم يتم توليده تلقائيا*

- *ملاحظات مهمة:*
  - *يمكن أن يكون هناك حقل `AUTO_INCREMENT` واحد فقط في الجدول*
  - *يجب أن يكون الحقل مفرداً (ليس جزءاً من مفتاح مركب فقط)*
  - *يجب أن يكون `NOT NULL` تلقائياً*
  - *الأفضل استخدامه مع `PRIMARY KEY` للأداء الأمثل*

```sql
-- الإضافة أثناء إنشاء الجدول:
CREATE TABLE my_table(
  id INT PRIMARY KEY AUTO_INCREMENT
);

-- الإضافة بعد إنشاء الجدول:
ALTER TABLE my_table
MODIFY id INT PRIMARY KEY AUTO_INCREMENT;

-- أو بدون تحديد القيد:
ALTER TABLE my_table
MODIFY id INT AUTO_INCREMENT;

-- عرض قيمة AUTO_INCREMENT الحالية
SHOW TABLE STATUS LIKE 'my_table';

-- الإزالة بعد الإضافة:
ALTER TABLE my_table
MODIFY id INT;
```

- *تحديد قيمة البداية:*

```sql
-- الإضافة أثناء إنشاء الجدول:
CREATE TABLE sequences(
    seq_id INT PRIMARY KEY AUTO_INCREMENT,
    seq_data VARCHAR(50)
) AUTO_INCREMENT = 1000;
-- سيبدأ الترقيم من 1000

-- الإضافة بعد إنشاء الجدول:
ALTER TABLE sequences AUTO_INCREMENT = 101;
```

--

- `AUTO_INCREMENT` *ليس* محصوراً على حقل `PRIMARY KEY` فقط، لكن له شروط واستخدامات محددة.

--

- الحقول التي يمكن أن تكون `AUTO_INCREMENT`:
  - *أي حقل مفرد* يمكن أن يكون `AUTO_INCREMENT` إذا كان:
    - من نوع عدد صحيح (`INT`, `SMALLINT`, `BIGINT`, etc.)
    - `UNIQUE` أو `PRIMARY KEY`

- *أمثلة على الاستخدامات المختلفة:*

```sql
-- 1. مع PRIMARY KEY (الأكثر شيوعاً)
CREATE TABLE users(
    id INT PRIMARY KEY AUTO_INCREMENT,
    username VARCHAR(50)
);

-- 2. مع UNIQUE KEY (يعمل أيضاً)
CREATE TABLE products(
    product_code INT UNIQUE AUTO_INCREMENT,
    product_name VARCHAR(100)
);

-- 3. مع KEY عادية (نادرة الاستخدام)
CREATE TABLE logs(
    log_id INT AUTO_INCREMENT,
    message TEXT,
    PRIMARY KEY (log_id, message(255))
);

-- 4. مع الحقول المركبة (Composite Keys) (استخدام متقدم)
CREATE TABLE order_items(
    order_id INT,
    item_id INT AUTO_INCREMENT,
    product_name VARCHAR(100),
    PRIMARY KEY (order_id, item_id)
);
-- يعمل لأن item_id جزء من PRIMARY KEY
```

--

- *ما لا يعمل:*

```sql
-- ❌ لا يعمل - ليس UNIQUE
CREATE TABLE test1(
    id INT AUTO_INCREMENT,  -- Error
    name VARCHAR(50)
);

-- ❌ لا يعمل - ليس مفتاحاً
CREATE TABLE test2(
    code INT AUTO_INCREMENT, -- Error
    description VARCHAR(100)
);
```

--

*مقارنة بين الاستخدامات:*

| الحقل | هل يعمل؟ | السبب |
|-------|----------|--------|
| `id INT PRIMARY KEY AUTO_INCREMENT` | ✅ | مفتاح رئيسي |
| `code INT UNIQUE AUTO_INCREMENT` | ✅ | فريد |
| `num INT AUTO_INCREMENT` | ❌ | ليس مفتاحاً أو فريداً |
| `seq INT KEY AUTO_INCREMENT` | ✅ | مفتاح |

--

*أمثلة عملية:*

```sql
-- مثال 1: مع UNIQUE
CREATE TABLE categories(
    cat_id INT UNIQUE AUTO_INCREMENT,
    cat_name VARCHAR(50) NOT NULL
);

INSERT INTO categories (cat_name) VALUES ('إلكترونيات');
INSERT INTO categories (cat_name) VALUES ('ملابس');
-- النتيجة: (1, 'إلكترونيات'), (2, 'ملابس')

-- مثال 2: مع PRIMARY KEY مركب
CREATE TABLE order_details(
    order_id INT,
    detail_id INT AUTO_INCREMENT,
    product_id INT,
    quantity INT,
    PRIMARY KEY (order_id, detail_id)
);

INSERT INTO order_details (order_id, product_id, quantity) VALUES (100, 1, 2);
INSERT INTO order_details (order_id, product_id, quantity) VALUES (100, 2, 1);
-- النتيجة: (100, 1, 1, 2), (100, 2, 2, 1)
```

###### `id SERIAL`

هو اختصار لـ:

```sql
id BIGINT UNSIGNED NOT NULL AUTO_INCREMENT UNIQUE
```

أي أن:

`SERIAL` = نوع `BIGINT UNSIGNED`
ومعه القيود: `NOT NULL` + `AUTO_INCREMENT` + `UNIQUE`
ملاحظة: رغم وجود `SERIAL،` إلا أن المطورين عادة يفضّلون كتابة النوع والقيود يدويًا (مثل `INT AUTO_INCREMENT PRIMARY KEY`) لأنها أوضح وأكثر تحكمًا.

مثال:

```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY
  username TEXT NOT NULL
);
```

--

##### مثال كامل

```sql
-- إنشاء جدول الأقسام (الجدول المرجعي)
CREATE TABLE departments(
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100) NOT NULL UNIQUE,
    manager_id INT,
    budget DECIMAL(12,2) CHECK (budget >= 0),
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-- إنشاء جدول الموظفين
CREATE TABLE employees(
    id INT PRIMARY KEY AUTO_INCREMENT,
    username VARCHAR(255) NOT NULL UNIQUE,
    email VARCHAR(255) UNIQUE NOT NULL,
    age INT NOT NULL CHECK (age >= 18 AND age <= 65),
    department_id INT NOT NULL,
    salary DECIMAL(10,2) NOT NULL CHECK (salary > 0 AND salary <= 100000),
    status VARCHAR(20) DEFAULT 'نشط' CHECK (status IN ('نشط', 'غير نشط', 'إجازة')),
    hire_date DATE DEFAULT (CURRENT_DATE),
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    
    -- المفتاح الخارجي مع خيارات ON DELETE و ON UPDATE
    FOREIGN KEY (department_id) 
        REFERENCES departments(id)
        ON DELETE RESTRICT
        ON UPDATE CASCADE
);

-- إضافة القيود بعد الإنشاء مع خيارات متقدمة
ALTER TABLE employees 
ADD CONSTRAINT uk_employee_username UNIQUE (username);

ALTER TABLE employees 
ADD CONSTRAINT chk_employee_salary_range 
CHECK (salary >= 1000 AND salary <= 50000);

ALTER TABLE employees 
ADD CONSTRAINT chk_employee_email_format 
CHECK (email LIKE '%@%.%'); -- يبدأ بـ (@) وفي الوسط (.)

-- إضافة مفتاح خارجي إضافي
ALTER TABLE departments 
ADD CONSTRAINT fk_department_manager
FOREIGN KEY (manager_id) 
REFERENCES employees(id)
ON DELETE SET NULL
ON UPDATE CASCADE;

-- إضافة قيود DEFAULT متقدمة
ALTER TABLE employees 
ALTER hire_date SET DEFAULT (CURRENT_DATE);

ALTER TABLE employees 
MODIFY created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP NOT NULL;

-- إزالة القيود مع الأمثلة المحدثة
-- إزالة NOT NULL
ALTER TABLE employees MODIFY username VARCHAR(255) NULL;

-- إزالة UNIQUE
ALTER TABLE employees DROP INDEX uk_employee_username;

-- إزالة CHECK
ALTER TABLE employees DROP CONSTRAINT chk_employee_salary_range;

-- إزالة DEFAULT
ALTER TABLE employees ALTER status DROP DEFAULT;

-- إزالة FOREIGN KEY
ALTER TABLE employees DROP FOREIGN KEY employees_ibfk_1;

-- إزالة PRIMARY KEY
ALTER TABLE employees DROP PRIMARY KEY;

-- التحقق من القيود المحدثة
-- عرض هيكل الجدول
DESCRIBE employees;

-- عرض جميع القيود
SELECT 
    CONSTRAINT_NAME,
    CONSTRAINT_TYPE,
    TABLE_NAME
FROM INFORMATION_SCHEMA.TABLE_CONSTRAINTS 
WHERE TABLE_NAME IN ('employees', 'departments');

-- عرض معلومات المفاتيح الخارجية
SELECT
    TABLE_NAME,
    COLUMN_NAME,
    CONSTRAINT_NAME,
    REFERENCED_TABLE_NAME,
    REFERENCED_COLUMN_NAME
FROM INFORMATION_SCHEMA.KEY_COLUMN_USAGE
WHERE REFERENCED_TABLE_NAME IS NOT NULL;

-- عرض قيود CHECK
SELECT 
    CONSTRAINT_NAME,
    CHECK_CLAUSE
FROM INFORMATION_SCHEMA.CHECK_CONSTRAINTS
WHERE TABLE_NAME = 'employees';

-- 🎯 مثال تطبيقي كامل محدث

-- إنشاء جدول الطلاب مع جميع القيود المطلوبة
CREATE TABLE students(
    id INT PRIMARY KEY AUTO_INCREMENT,
    student_code VARCHAR(20) UNIQUE NOT NULL,
    name VARCHAR(255) NOT NULL,
    email VARCHAR(255) UNIQUE NOT NULL,
    age INT NOT NULL CHECK (age BETWEEN 15 AND 25),
    grade VARCHAR(10) DEFAULT 'غير مكتمل' CHECK (grade IN ('ممتاز', 'جيد جداً', 'جيد', 'مقبول', 'غير مكتمل')),
    gpa DECIMAL(3,2) CHECK (gpa >= 0 AND gpa <= 4.0),
    department_id INT NOT NULL,
    enrollment_date DATE DEFAULT (CURRENT_DATE),
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    
    -- المفتاح الخارجي
    FOREIGN KEY (department_id) 
        REFERENCES departments(id)
        ON DELETE CASCADE
        ON UPDATE CASCADE
);

-- إنشاء جدول المساقات
CREATE TABLE courses(
    id INT PRIMARY KEY AUTO_INCREMENT,
    code VARCHAR(20) UNIQUE NOT NULL,
    name VARCHAR(255) NOT NULL,
    credits INT NOT NULL CHECK (credits BETWEEN 1 AND 5),
    department_id INT NOT NULL,
    max_students INT DEFAULT 30 CHECK (max_students > 0),
    is_active BOOLEAN DEFAULT TRUE,
    
    FOREIGN KEY (department_id) 
        REFERENCES departments(id)
        ON DELETE RESTRICT
        ON UPDATE CASCADE
);

-- إنشاء جدول تسجيل المساقات (جدول ارتباطي)
CREATE TABLE student_courses(
    student_id INT NOT NULL,
    course_id INT NOT NULL,
    enrollment_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    grade DECIMAL(4,2) CHECK (grade >= 0 AND grade <= 100),
    status VARCHAR(20) DEFAULT 'مسجل' CHECK (status IN ('مسجل', 'منسحب', 'مكتمل')),
    
    PRIMARY KEY (student_id, course_id),
    
    FOREIGN KEY (student_id) 
        REFERENCES students(id)
        ON DELETE CASCADE
        ON UPDATE CASCADE,
        
    FOREIGN KEY (course_id) 
        REFERENCES courses(id)
        ON DELETE RESTRICT
        ON UPDATE CASCADE
);

-- إضافة قيود إضافية بعد الإنشاء
ALTER TABLE students 
ADD CONSTRAINT chk_student_email_domain 
CHECK (email LIKE '%@university.edu');

ALTER TABLE courses 
ADD CONSTRAINT chk_course_credits 
CHECK (credits IN (1, 2, 3, 4, 5));

-- إضافة قيود DEFAULT متقدمة
ALTER TABLE student_courses 
ALTER enrollment_date SET DEFAULT (CURRENT_TIMESTAMP);

-- التحقق من الهياكل والقيود
DESCRIBE students;
DESCRIBE courses;
DESCRIBE student_courses;

-- عرض جميع القيود في قاعدة البيانات
SELECT 
    TABLE_NAME,
    CONSTRAINT_NAME,
    CONSTRAINT_TYPE
FROM INFORMATION_SCHEMA.TABLE_CONSTRAINTS 
WHERE TABLE_SCHEMA = DATABASE()
ORDER BY TABLE_NAME, CONSTRAINT_TYPE;

-- عرض المفاتيح الخارجية بالتفصيل
SELECT
    rc.CONSTRAINT_NAME,
    rc.TABLE_NAME,
    kcu.COLUMN_NAME,
    rc.REFERENCED_TABLE_NAME,
    rc.REFERENCED_COLUMN_NAME,
    rc.DELETE_RULE,
    rc.UPDATE_RULE
FROM INFORMATION_SCHEMA.REFERENTIAL_CONSTRAINTS rc
JOIN INFORMATION_SCHEMA.KEY_COLUMN_USAGE kcu
    ON rc.CONSTRAINT_NAME = kcu.CONSTRAINT_NAME
WHERE rc.CONSTRAINT_SCHEMA = DATABASE();
```

--

#### Relationships - العلاقات

*شرح نظرى مبسط:*

- `One to One Relation`: علاقة سجل جدول بسجل جدول
  - مثال: كل شخص له بطاقة شخصية واحدة خاصة به وهذه البطاقة لا يمكن مشاركتها مع شخص آخر

- `One to Many Relation`: علاقة سجل جدول بعدة سجلات جدول
  - مثال: كل بطاقة لها عدة إصدارات خاصة بها وهذه الإصدارات لا يمكن مشاركتها مع بطاقة أخرى

- `Many to Many Relation`: علاقة عدة سجلات جدول بعدة سجلات جدول
  - مثال: كل شخص يمكنه السفر لعدة دول وكل الدولة يمكن أن يسافرها عدة أشخاص

##### 1. One to One Relation (علاقة واحد لواحد)

*الوصف:* كل سجل في الجدول (أ) يرتبط بسجل واحد فقط في الجدول (ب)، والعكس صحيح.

*مثال عملي:* نظام للموظفين حيث لكل موظف *سجل راتب واحد* خاص به فقط.

```sql
-- جدول الموظفين
CREATE TABLE Employees (
    employee_id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100) NOT NULL,
    email VARCHAR(100) UNIQUE NOT NULL
);

-- جدول تفاصيل الرواتب (مرتبط one-to-one)
CREATE TABLE SalaryDetails (
    employee_id INT PRIMARY KEY, -- نفس مفتاح الموظف
    salary DECIMAL(10, 2) NOT NULL,
    bank_account_number VARCHAR(20),
    FOREIGN KEY (employee_id) REFERENCES Employees(employee_id)
);
```

*الاستعلام لجلب البيانات:*

```sql
SELECT e.name, s.salary
FROM Employees e
INNER JOIN SalaryDetails s ON e.employee_id = s.employee_id;
```

##### 2. One to Many Relation (علاقة واحد لكثير)

*الوصف:* سجل واحد في الجدول (أ) يمكن أن يرتبط بعدة سجلات في الجدول (ب). لكن السجل في الجدول (ب) يرتبط بسجل واحد فقط في الجدول (أ). هذا هو *النوع الأكثر شيوعًا*.

*مثال عملي:* نظام للمدونة، حيث *مقال واحد* يمكن أن يحتوي على *عدة تعليقات*.

```sql
-- جدول المقالات
CREATE TABLE Articles (
    article_id INT PRIMARY KEY AUTO_INCREMENT,
    title VARCHAR(255) NOT NULL,
    content TEXT
);

-- جدول التعليقات (مرتبط one-to-many مع المقالات)
CREATE TABLE Comments (
    comment_id INT PRIMARY KEY AUTO_INCREMENT,
    article_id INT NOT NULL, -- المفتاح الخارجي الذي يشير للمقال
    author_name VARCHAR(100),
    comment_text TEXT,
    FOREIGN KEY (article_id) REFERENCES Articles(article_id)
);
```

*الاستعلام لجلب جميع التعليقات لمقال معين (مثلاً المقال رقم 5):*

```sql
SELECT a.title, c.author_name, c.comment_text
FROM Articles a
INNER JOIN Comments c ON a.article_id = c.article_id
WHERE a.article_id = 5;
```

---

##### 3. Many to Many Relation (علاقة كثير لكثير)

*الوصف:* عدة سجلات في الجدول (أ) يمكن أن ترتبط بعدة سجلات في الجدول (ب)، والعكس صحيح. لتنفيذ هذه العلاقة، نحتاج إلى *جدول وسيط* (Junction Table).

*مثال عملي:* نظام للطلاب والمقررات الدراسية، حيث *الطالب الواحد يمكنه تسجيل عدة مقررات*، و *المقرر الواحد يمكن أن يسجله عدة طلاب*.

```sql
-- جدول الطلاب
CREATE TABLE Students (
    student_id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100) NOT NULL
);

-- جدول المقررات
CREATE TABLE Courses (
    course_id INT PRIMARY KEY AUTO_INCREMENT,
    course_name VARCHAR(100) NOT NULL
);

-- الجدول الوسيط لتنفيذ علاقة many-to-many
CREATE TABLE Student_Courses (
    student_id INT,
    course_id INT,
    enrollment_date DATE,
    PRIMARY KEY (student_id, course_id), -- المفتاح الأساسي مركب
    FOREIGN KEY (student_id) REFERENCES Students(student_id),
    FOREIGN KEY (course_id) REFERENCES Courses(course_id)
);
```

*الاستعلام لمعرفة المقررات التي سجلها طالب معين (مثلاً الطالب رقم 10):*

```sql
SELECT s.name, c.course_name
FROM Students s
INNER JOIN Student_Courses sc ON s.student_id = sc.student_id
INNER JOIN Courses c ON sc.course_id = c.course_id
WHERE s.student_id = 10;
```

*الاستعلام لمعرفة الطلاب المسجلين في مقرر معين (مثلاً مقرر "قواعد البيانات"):*

```sql
SELECT c.course_name, s.name
FROM Courses c
INNER JOIN Student_Courses sc ON c.course_id = sc.course_id
INNER JOIN Students s ON sc.student_id = s.student_id
WHERE c.course_name = 'قواعد البيانات';
```

--

| نوع العلاقة      | الوصف | المفتاح الخارجي | مثال |
|------------------|-------|-----------------|-------------|
| *One to One*   | سجل -> سجل | في الجدول الثانوي (غالباً Primary Key أيضاً) | `Employees` - `SalaryDetails` |
| *One to Many*  | سجل -> عدة سجلات | في الجدول الذي ينتمي للـ "Many" | `Articles` - `Comments` |
| *Many to Many* | عدة سجلات -> عدة سجلات | في *جدول وسيط* يربط between هما | `Students` - `Courses` (باستخدام `Student_Courses`) |

--

#### JOINs - الوصلات

- `JOINs` هي عمليات تستخدم لدمج بيانات من جدولين أو أكثر بناءً على عمود مشترك بينهما. هناك عدة أنواع من ال `JOINs`:

- أنواع `JOINs` الأساسية:
  - `INNER JOIN`
  - `LEFT JOIN`
  - `RIGHT JOIN`
  - `FULL OUTER JOIN`
  - `SELF JOIN`
  - `CROSS JOIN`

--

- إنشاء الجداول وإدراج البيانات:

```sql
-- جدول الأقسام
CREATE TABLE departments (
    department_id INT PRIMARY KEY AUTO_INCREMENT,
    department_name VARCHAR(100) NOT NULL
);

-- جدول الموظفين
CREATE TABLE employees (
    employee_id INT PRIMARY KEY AUTO_INCREMENT,
    employee_name VARCHAR(100) NOT NULL,
    department_id INT,
    manager_id INT,
    FOREIGN KEY (department_id) REFERENCES departments(department_id),
    FOREIGN KEY (manager_id) REFERENCES employees(employee_id) -- SELF JOIN
);

-- جدول العملاء
CREATE TABLE customers (
    customer_id INT PRIMARY KEY AUTO_INCREMENT,
    customer_name VARCHAR(100) NOT NULL
);

-- جدول الطلبات
CREATE TABLE orders (
    order_id INT PRIMARY KEY AUTO_INCREMENT,
    customer_id INT,
    order_date DATE,
    FOREIGN KEY (customer_id) REFERENCES customers(customer_id)
);

-- جداول للألوان والمقاسات (لـ CROSS JOIN)
CREATE TABLE sizes (
    size VARCHAR(10) PRIMARY KEY
);

CREATE TABLE colors (
    color VARCHAR(20) PRIMARY KEY
);
```

- إدراج البيانات التجريبية:

```sql
-- إدراج الأقسام
INSERT INTO departments (department_name) VALUES 
('المبيعات'),
('التسويق'),
('تكنولوجيا المعلومات'),
('الموارد البشرية');

-- إدراج الموظفين
INSERT INTO employees (employee_name, department_id, manager_id) VALUES 
('أحمد محمد', 1, NULL),
('فاطمة علي', 1, 1),
('خالد ابراهيم', 3, NULL),
('سارة عبدالله', 2, NULL),
('محمد حسن', NULL, 3), -- موظف بدون قسم
('ليلى كمال', 3, 3);

-- إدراج العملاء والطلبات
INSERT INTO customers (customer_name) VALUES 
('شركة الأمل'),
('مؤسسة النجاح'),
('شركة المستقبل');

INSERT INTO orders (customer_id, order_date) VALUES 
(1, '2024-01-15'),
(2, '2024-01-16'),
(1, '2024-01-17');

-- إدراج المقاسات والألوان
INSERT INTO sizes (size) VALUES 
('S'), ('M'), ('L'), ('XL');

INSERT INTO colors (color) VALUES 
('أحمر'), ('أزرق'), ('أخضر'), ('أسود');
```

--

##### 1. *INNER JOIN* - الربط الداخلي

- *هو النوع الافتراضي*

*يعيد فقط السجلات التي لها قيم مطابقة في كلا الجدولين:*

```sql
SELECT columns
FROM table1
INNER JOIN table2 ON table1.column = table2.column;

-- أو
SELECT columns
FROM table1
JOIN table2 ON table1.column = table2.column;
```

*مثال عملي:*

```sql
-- الموظفون الذين لديهم قسم
SELECT employees.employee_name, departments.department_name
FROM employees
INNER JOIN departments ON employees.department_id = departments.department_id;

-- Or
SELECT e.employee_name, d.department_name
FROM employees e
INNER JOIN departments d ON e.department_id = d.department_id;
```

*النتيجة:*

| الاسم الكامل    | القسم               |
|-----------------|---------------------|
| أحمد محمد      | المبيعات           |
| فاطمة علي      | المبيعات           |
| خالد ابراهيم   | تكنولوجيا المعلومات |
| سارة عبدالله   | التسويق            |
| ليلى كمال      | تكنولوجيا المعلومات |

##### 2. *LEFT JOIN* - الربط الأيسر

*يعيد جميع السجلات من الجدول الأيسر والسجلات المطابقة من الجدول الأيمن:*

```sql
SELECT columns
FROM table1
LEFT JOIN table2 ON table1.column = table2.column;
```

*مثال عملي:*

```sql
-- جميع الموظفين حتى الذين ليس لديهم قسم
SELECT employees.employee_name, departments.department_name
FROM employees
LEFT JOIN departments ON employees.department_id = departments.department_id;

-- Or
SELECT e.employee_name, d.department_name
FROM employees e
LEFT JOIN departments d ON e.department_id = d.department_id;
```

*النتيجة:*

| الاسم الكامل    | القسم               |
|-----------------|---------------------|
| أحمد محمد      | المبيعات           |
| فاطمة علي      | المبيعات           |
| خالد ابراهيم   | تكنولوجيا المعلومات |
| سارة عبدالله   | التسويق            |
| محمد حسن       | NULL                |
| ليلى كمال      | تكنولوجيا المعلومات |

##### 3. *RIGHT JOIN* - الربط الأيمن

*يعيد جميع السجلات من الجدول الأيمن والسجلات المطابقة من الجدول الأيسر:*

```sql
SELECT columns
FROM table1
RIGHT JOIN table2 ON table1.column = table2.column;
```

*مثال عملي:*

```sql
-- جميع الأقسام حتى التي ليس لها موظفين
SELECT employees.employee_name, departments.department_name
FROM employees
RIGHT JOIN departments ON employees.department_id = departments.department_id;

-- Or
SELECT e.employee_name, d.department_name
FROM employees e
RIGHT JOIN departments d ON e.department_id = d.department_id;
```

*النتيجة:*

| الاسم الكامل    | القسم               |
|-----------------|---------------------|
| أحمد محمد      | المبيعات           |
| فاطمة علي      | المبيعات           |
| سارة عبدالله   | التسويق            |
| خالد ابراهيم   | تكنولوجيا المعلومات |
| ليلى كمال      | تكنولوجيا المعلومات |
| NULL           | الموارد البشرية    |

##### 4. *FULL OUTER JOIN (UNION)* - الربط الخارجي الكامل

*يعيد جميع السجلات عندما يكون هناك تطابق في أي من الجدولين:*

```sql
-- ملاحظة: MySQL لا تدعم FULL OUTER JOIN مباشرة
-- نستخدم UNION بين LEFT و RIGHT JOIN
SELECT columns FROM table1 LEFT JOIN table2 ON condition
UNION
SELECT columns FROM table1 RIGHT JOIN table2 ON condition;

-- ALL: تعرض السجلات المكررة
SELECT columns FROM table1
UNION ALL
SELECT columns FROM table1;
```

*مثال عملي:*

```sql
SELECT e.employee_name, d.department_name
FROM employees e
LEFT JOIN departments d ON e.department_id = d.department_id
UNION
SELECT e.employee_name, d.department_name
FROM employees e
RIGHT JOIN departments d ON e.department_id = d.department_id;
```

*النتيجة:*

| الاسم الكامل    | القسم               |
|-----------------|---------------------|
| أحمد محمد      | المبيعات           |
| فاطمة علي      | المبيعات           |
| خالد ابراهيم   | تكنولوجيا المعلومات |
| سارة عبدالله   | التسويق            |
| محمد حسن       | NULL                |
| ليلى كمال      | تكنولوجيا المعلومات |
| NULL           | الموارد البشرية    |

##### 5. *SELF JOIN* - الربط الذاتي

```sql
-- ربط الجدول مع نفسه
SELECT e1.employee_name as employee, e2.employee_name as manager
FROM employees e1
LEFT JOIN employees e2 ON e1.manager_id = e2.employee_id;
```

*النتيجة:*

| الموظف         | المدير            |
|----------------|-------------------|
| أحمد محمد     | NULL              |
| فاطمة علي     | أحمد محمد        |
| خالد ابراهيم  | NULL              |
| سارة عبدالله  | NULL              |
| محمد حسن      | خالد ابراهيم      |
| ليلى كمال     | خالد ابراهيم      |

##### 6. *CROSS JOIN* - الربط التبادلي

```sql
-- ينتج جميع التوليفات الممكنة (الضرب الديكارتي)
SELECT sizes.size, colors.color
FROM sizes
CROSS JOIN colors;
```

*النتيجة: (16 سجل - 4 مقاسات × 4 ألوان):*

```text
S | أحمر
S | أزرق
S | أخضر
S | أسود
M | أحمر
M | أزرق
... إلخ
```

- تحذير مهم حول `CROSS JOIN`:

```sql
-- ⚠️ احذر: هذا يمكن أن ينتج عدد هائل من السجلات
SELECT * FROM table1 CROSS JOIN table2;

-- مثال: إذا كان table1 به 1000 سجل و table2 به 1000 سجل
-- النتيجة: 1,000,000 سجل!
```

- مثال تحذيري لـ `CROSS JOIN` (غير مرغوب):

```sql
-- هذا سيعيد ضرب جميع السجلات (خطأ شائع)
SELECT * FROM customers, orders; -- بدون شرط WHERE أو ON

-- الصحيح:
SELECT * FROM customers CROSS JOIN orders; -- نادر الاستخدام
```

--

##### أمثلة عملية مفصلة لكل نوع

--

*أمثلة عملية شاملة:*

لنفترض لدينا قاعدة بيانات لمتجر:

```sql
-- جدول العملاء
CREATE TABLE customers (
    customer_id INT PRIMARY KEY,
    customer_name VARCHAR(100),
    city VARCHAR(50)
);

-- إدراج بيانات العملاء
INSERT INTO customers (customer_id, customer_name, city) VALUES
(1, 'أحمد محمد', 'الرياض'),
(2, 'فاطمة علي', 'جدة'),
(3, 'خالد السعدي', 'الرياض'),
(4, 'نورة القحطاني', 'الدمام'),
(5, 'محمد الغامدي', 'مكة');

-----------------------------

-- جدول الطلبات
CREATE TABLE orders (
    order_id INT PRIMARY KEY,
    customer_id INT,
    order_date DATE,
    amount DECIMAL(10,2),
    FOREIGN KEY (customer_id) REFERENCES customers(customer_id)
);

-- إدراج بيانات الطلبات
INSERT INTO orders (order_id, customer_id, order_date, amount) VALUES
(1001, 1, '2024-01-15', 5700.00),
(1002, 2, '2024-01-16', 2200.00),
(1003, 1, '2024-01-18', 300.00),
(1004, 3, '2024-01-20', 1800.00),
(1005, 4, '2024-01-22', 150.00);

-----------------------------

-- جدول المنتجات
CREATE TABLE products (
    product_id INT PRIMARY KEY,
    product_name VARCHAR(100),
    price DECIMAL(10,2)
);

-- إدراج بيانات المنتجات
INSERT INTO products (product_id, product_name, price) VALUES
(101, 'لابتوب ديل', 3500.00),
(102, 'هاتف سامسونج', 2200.00),
(103, 'تابلت أبل', 1800.00),
(104, 'سماعات لاسلكية', 300.00),
(105, 'لوحة مفاتيح', 150.00);

-----------------------------

-- جدول عناصر الطلبات
CREATE TABLE order_items (
    order_id INT,
    product_id INT,
    quantity INT,
    PRIMARY KEY (order_id, product_id),
    FOREIGN KEY (order_id) REFERENCES orders(order_id),
    FOREIGN KEY (product_id) REFERENCES products(product_id)
);

-- إدراج بيانات عناصر الطلبات
INSERT INTO order_items (order_id, product_id, quantity) VALUES
(1001, 101, 1),
(1001, 104, 1),
(1002, 102, 1),
(1003, 104, 1),
(1004, 103, 1),
(1005, 105, 1);

-----------------------------

CREATE TABLE employees (
    employee_id INT PRIMARY KEY,
    employee_name VARCHAR(100),
    manager_id INT,
    FOREIGN KEY (manager_id) REFERENCES employees(employee_id)
);

-- إدراج بيانات الموظفين
INSERT INTO employees (employee_id, employee_name, manager_id) VALUES
(1, 'سعيد الحربي', NULL),
(2, 'ليلى العتيبي', 1),
(3, 'عمر النجاري', 1),
(4, 'هديل الشمري', 2),
(5, 'بدر الرشيد', 3);
```

- الرسم البياني للعلاقات بين الجداول

```text
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   customers     │    │     orders      │    │   order_items   │
├─────────────────┤    ├─────────────────┤    ├─────────────────┤
│ customer_id (PK)│◄───│ customer_id (FK)│    │ order_id (FK,PK)│
│ customer_name   │    │ order_id (PK)   │◄───│ product_id(FK,PK)│
│ city            │    │ order_date      │    │ quantity        │
└─────────────────┘    │ amount          │    └────────┬────────┘
                       └─────────────────┘             │
                                                       │
┌─────────────────┐                                    │
│   employees     │    ┌─────────────────┐             │
├─────────────────┤    │    products     │             │
│ employee_id (PK)│    ├─────────────────┤             │
│ employee_name   │    │ product_id (PK) │◄────────────┘
│ manager_id (FK) │    │ product_name    │
└─────────────────┘    │ price           │
          │            └─────────────────┘
          │
          └─────┘ (العلاقة الذاتية - self join)
```

- شرح العلاقات بالتفصيل:

1. **علاقة customers ↔ orders**

   - **one-to-many**
   - عميل واحد يمكن أن يكون له عدة طلبات
   - `customers.customer_id (PK)` → `orders.customer_id (FK)`

2. **علاقة orders ↔ order_items**

   - **one-to-many**
   - طلب واحد يمكن أن يحتوي على عدة عناصر
   - `orders.order_id (PK)` → `order_items.order_id (FK)`

3. **علاقة products ↔ order_items**

   - **one-to-many**
   - منتج واحد يمكن أن يظهر في عدة عناصر طلبات
   - `products.product_id (PK)` → `order_items.product_id (FK)`

4. **علاقة employees الذاتية**

   - **one-to-many** (ذاتية)
   - موظف واحد يمكن أن يكون مديراً لعدة موظفين
   - `employees.employee_id (PK)` → `employees.manager_id (FK)`

- المفاتيح الأساسية والأجنبية

| الجدول      | المفتاح الأساسي         | المفاتيح الأجنبية        |
|-------------|--------------------------|--------------------------|
| customers   | `customer_id`            | -                        |
| orders      | `order_id`               | `customer_id`            |
| products    | `product_id`             | -                        |
| order_items | `(order_id, product_id)` | `order_id`, `product_id` |
| employees   | `employee_id`            | `manager_id`             |

- مثال على تدفق البيانات:

عميل (customers)
    ↓
يقدم طلب (orders)
    ↓
يحتوي على عناصر (order_items)
    ↓
ترتبط بمنتجات (products)

- أمثلة `JOINs` متعددة:

**1. INNER JOIN بسيط:**

```sql
-- العملاء الذين قاموا بطلبات
SELECT c.customer_name, o.order_date, o.amount
FROM customers c
INNER JOIN orders o ON c.customer_id = o.customer_id;
```

*النتيجة:*

| customer_name   | order_date | amount    |
|-----------------|------------|-----------|
| أحمد محمد      | 2024-01-15 | 5700.00   |
| فاطمة علي      | 2024-01-16 | 2200.00   |
| أحمد محمد      | 2024-01-18 | 300.00    |
| خالد السعدي    | 2024-01-20 | 1800.00   |
| نورة القحطاني  | 2024-01-22 | 150.00    |

**2. LEFT JOIN:**

```sql
-- جميع العملاء مع طلباتهم (حتى الذين لم يطلبوا)
SELECT c.customer_name, o.order_date, o.amount
FROM customers c
LEFT JOIN orders o ON c.customer_id = o.customer_id;
```

*النتيجة:*

| customer_name   | order_date | amount    |
|-----------------|------------|-----------|
| أحمد محمد      | 2024-01-15 | 5700.00   |
| أحمد محمد      | 2024-01-18 | 300.00    |
| فاطمة علي      | 2024-01-16 | 2200.00   |
| خالد السعدي    | 2024-01-20 | 1800.00   |
| نورة القحطاني  | 2024-01-22 | 150.00    |
| محمد الغامدي   | NULL       | NULL      |

**3. JOIN مع ثلاثة جداول:**

```sql
-- تفاصيل الطلب مع معلومات العميل والمنتجات
SELECT 
    c.customer_name,
    o.order_date,
    p.product_name,
    oi.quantity,
    (oi.quantity * p.price) as total_price
FROM orders o
INNER JOIN customers c ON o.customer_id = c.customer_id
INNER JOIN order_items oi ON o.order_id = oi.order_id
INNER JOIN products p ON oi.product_id = p.product_id;
```

*النتيجة:*

| اسم العميل      | تاريخ الطلب   | المنتج           | الكمية | السعر الإجمالي |
|-----------------|---------------|------------------|--------|---------------|
| أحمد محمد      | 2024-01-15    | لابتوب ديل       | 1      | 3500.00       |
| أحمد محمد      | 2024-01-15    | سماعات لاسلكية   | 1      | 300.00        |
| فاطمة علي      | 2024-01-16    | هاتف سامسونج    | 1      | 2200.00       |
| أحمد محمد      | 2024-01-18    | سماعات لاسلكية   | 1      | 300.00        |
| خالد السعدي    | 2024-01-20    | تابلت أبل       | 1      | 1800.00       |
| نورة القحطاني  | 2024-01-22    | لوحة مفاتيح     | 1      | 150.00        |

**4. JOIN مع WHERE clause:**

```sql
-- طلبات العملاء من مدينة معينة
SELECT c.customer_name, o.order_date, o.amount
FROM customers c
INNER JOIN orders o ON c.customer_id = o.customer_id
WHERE c.city = 'الرياض';
```

*النتيجة:*

| customer_name   | order_date | amount    |
|-----------------|------------|-----------|
| أحمد محمد      | 2024-01-15 | 5700.00   |
| أحمد محمد      | 2024-01-18 | 300.00    |
| خالد السعدي    | 2024-01-20 | 1800.00   |

**5. JOIN مع GROUP BY:**

تستخدم `GROUP BY` لتجميع الصفوف التي لها قيم متطابقة في عمود أو أكثر في مجموعات

```sql
-- إجمالي المبيعات لكل عميل
SELECT 
    c.customer_name,
    SUM(o.amount) as total_spent
FROM customers c
LEFT JOIN orders o ON c.customer_id = o.customer_id
GROUP BY c.customer_id, c.customer_name;
```

*النتيجة:*

| customer_name   | total_spent |
|-----------------|-------------|
| أحمد محمد      | 6000.00     |
| فاطمة علي      | 2200.00     |
| خالد السعدي    | 1800.00     |
| نورة القحطاني  | 150.00      |
| محمد الغامدي   | NULL        |

**6. SELF JOIN (ربط الجدول مع نفسه):**

```sql
-- الموظفون ومديروهم
SELECT 
    e.employee_name as employee,
    m.employee_name as manager
FROM employees e
LEFT JOIN employees m ON e.manager_id = m.employee_id;
```

*النتيجة:*

| employee      | manager       |
|---------------|---------------|
| سعيد الحربي  | NULL          |
| ليلى العتيبي | سعيد الحربي  |
| عمر النجاري  | سعيد الحربي  |
| هديل الشمري  | ليلى العتيبي |
| بدر الرشيد   | عمر النجاري  |

--

- مثال آخر مع البيانات:

```sql
-- إنشاء الجداول
CREATE TABLE employees (
    id INT PRIMARY KEY,
    name VARCHAR(100),
    dept_id INT,
    manager_id INT
);

CREATE TABLE departments (
    id INT PRIMARY KEY,
    department_name VARCHAR(100)
);

CREATE TABLE projects (
    id INT PRIMARY KEY,
    project_name VARCHAR(100)
);

CREATE TABLE employee_projects (
    emp_id INT,
    project_id INT
);
```

1. *INNER JOIN عملي:*

    ```sql
    -- الموظفون الذين لديهم أقسام فقط
    SELECT e.name, d.department_name
    FROM employees e
    INNER JOIN departments d ON e.dept_id = d.id;
    ```

2. *LEFT JOIN عملي:*

    ```sql
    -- جميع الموظفين مع أقسامهم (حتى بدون قسم)
    SELECT e.name, d.department_name
    FROM employees e
    LEFT JOIN departments d ON e.dept_id = d.id;
    ```

3. *RIGHT JOIN عملي:*

    ```sql
    -- جميع الأقسام مع موظفيها (حتى الأقسام الفارغة)
    SELECT e.name, d.department_name
    FROM employees e
    RIGHT JOIN departments d ON e.dept_id = d.id;
    ```

4. *FULL OUTER JOIN عملي:*

    ```sql
    -- جميع الموظفين وجميع الأقسام
    SELECT e.name, d.department_name
    FROM employees e
    LEFT JOIN departments d ON e.dept_id = d.id
    UNION
    SELECT e.name, d.department_name
    FROM employees e
    RIGHT JOIN departments d ON e.dept_id = d.id;
    ```

5. *SELF JOIN عملي:*

    ```sql
    -- هيكل الإدارة: الموظفون ومديروهم
    SELECT 
        emp.name as employee_name,
        mgr.name as manager_name
    FROM employees emp
    LEFT JOIN employees mgr ON emp.manager_id = mgr.id;
    ```

6. *CROSS JOIN عملي:*

    ```sql
    -- إنشاء جميع التركيبات الممكنة (مفيد للتقارير الشاملة)
    SELECT 
        d.department_name,
        p.project_name
    FROM departments d
    CROSS JOIN projects p;
    ```

--

- نصائح مهمة:

1. **استخدم Aliases** لأسماء الجداول لتقصير الاستعلام
2. **حدد الأعمدة بوضوح** باستخدام النقطة (table.column)
3. **استخدم WHERE** لتصفية النتائج بعد ال JOIN
4. **INDEX** الأعمدة المستخدمة في ال ON لتحسين الأداء
5. **تجنب CARTESIAN PRODUCT** (الضرب الديكارتي) بدون شرط ON

- الفروق بين جميع الأنواع:

| النوع               | الوصف                           | الاستخدام الشائع     |
|---------------------|----------------------------------|----------------------|
| **INNER JOIN**      | السجلات المطابقة فقط             | البيانات المترابطة |
| **LEFT JOIN**       | كل اليسار + المطابقة من اليمين | التقارير الشاملة    |
| **RIGHT JOIN**      | كل اليمين + المطابقة من اليسار | نادر الاستخدام       |
| **FULL OUTER JOIN** | جميع السجلات من كلا الجدولين     | مقارنة شاملة         |
| **SELF JOIN**       | ربط الجدول مع نفسه              | الهياكل الهرمية     |
| **CROSS JOIN**      | جميع التوليفات الممكنة         | البيانات المرجعية   |

--

#### Advanced Select - الاختيار المتقدم

##### Logical Operators - العمليات المنطقية

- `AND`: يجب تنفيذ كل الشروط
- `OR`: يمكن تنفيذ أحد الشروط
- `NOT`: مخالفة الشرط
- `BETWEEN`: البحث بين قيمتين
- `IN`: تنفيذ داخل الشرط

```sql
CREATE TABLE users(
  id INT PRIMARY KEY AUTO_INCREMENT,
  first_name VARCHAR(50),
  last_name VARCHAR(50),
  country VARCHAR(50)
);

INSERT INTO users(first_name, last_name, country) VALUES
('Ali', 'Mohammed', 'Egypt'),
('Ola', 'Sayed', 'Egypt'),
('Sammy', 'Mohammed', 'Egypt'),
('Diaa', 'Sayed', 'Egypt'),
('Saad', 'Mohammed', 'Iraq');

-- AND
SELECT * FROM users WHERE last_name = 'Mohammed' AND country = 'Egypt';
-- النتائج:
-- 1, Ali, Mohammed, Egypt
-- 3, Sammy, Mohammed, Egypt

-- OR
SELECT * FROM users WHERE last_name = 'Sayed' OR country = 'Iraq';
-- النتائج:
-- 2, Ola, Sayed, Egypt
-- 4, Diaa, Sayed, Egypt
-- 5, Saad, Mohammed, Iraq

-- NOT
SELECT * FROM users WHERE NOT country = 'Iraq';
-- النتائج:
-- 1, Ali, Mohammed, Egypt
-- 2, Ola, Sayed, Egypt
-- 3, Sammy, Mohammed, Egypt
-- 4, Diaa, Sayed, Egypt

-- BETWEEN
--  بدلا من:
SELECT * FROM users WHERE id >= 1 AND id <= 4;
-- نكتب:
SELECT * FROM users WHERE id BETWEEN 1 AND 4;

-- IN
-- بدلا من:
SELECT * FROM users WHERE id = 1 OR id = 3 OR id = 4;
-- نكتب:
SELECT * FROM users WHERE id IN (1, 3, 4);

-- البحث عن عنصر به حرف h بعده قيم محددة
CREATE TABLE names(username VARCHAR(50));
INSERT INTO names VALUES
('Ahmed'),
('Khaled'),
('Shady'),
('Aya'),
('Asmaa');

SELECT * FROM names WHERE username REGEXP '.*h.*[mly].*';
-- Ahmed
-- Khaled
-- Shady
```

- `Comparisons`: المقارنات

```sql
SELECT 1 > 2; -- هل 1 أكبر من 2: 0 (False)
SELECT 1 < 2; -- هل 1 أصغر من 2: 1 (True)
SELECT 10 = 10; -- هل 10 تساوي 10: 1 (True)
SELECT 5 != 10; -- هل 10 لا تساوي 10: 0 (False)
SELECT 5 <> 10; -- هل 10 لا تساوي 10: 0 (False)
```

##### Calculations Operations - العمليات الحسابية

```sql
SELECT 1, 2; -- عرض قيم معينة في حقول
SELECT 1 AS ONE, 2 AS TOW; -- AS: تخصيص اسم للحقل
SELECT 1 + 2; -- جمع
SELECT 1 - 2; -- طرح
SELECT 1 * 2; -- ضرب
SELECT 1 / 2; -- قسمة
SELECT 10 % 3; -- الباقي من القسمة
```

##### Wildcards - أحرف البدل

- *هي رموز خاصة تُستخدم لتمثيل حرف واحد أو أكثر في عملية بحث أو مطابقة نمط*

- `LIKE`: أداة التمثيل
  - `%`: تمثيل أي عدد من الحروف
  - `_`: تمثيل حرف واحد
  - `[]`: تمثل حروف معينة (في `SQL Server`)

```sql
CREATE TABLE names_table(name VARCHAR(50));
INSERT INTO names_table VALUES
('Ali'), ('Alaa'), ('Ahmed'), ('Ola'), ('Mohamed'), ('Mahmoud');

-- (%)
SELECT * FROM names_table WHERE name LIKE 'A%';
-- النتائج:
-- Ali
-- Alaa
-- Ahmed
SELECT * FROM names_table WHERE name LIKE '%l%';
-- النتائج:
-- Ali
-- Alaa
-- Ola
SELECT * FROM names_table WHERE name LIKE '%d';
-- النتائج:
-- Ahmed
-- Mohamed
-- Mahmoud

-- SQL Server
SELECT * FROM names_table WHERE name LIKE '%[lm]a%';
-- Alaa
-- Ola
-- Mahmoud

-- (_)
SELECT * FROM names_table WHERE name LIKE '_h%';
-- النتائج:
-- Ahmed
SELECT * FROM names_table WHERE name LIKE '__h%';
-- النتائج:
-- Mohamed
-- Mahmoud

-- SQL Server
SELECT * FROM names WHERE username NOT LIKE '__[a-i]%';  -- Ahmed
```

##### LIMITs - الحدود

- *البحث عند حد معين*
- *نقطة البداية الافتراضية تبدأ من الفهرس (0)*

```sql
SELECT * FROM names_table LIMIT 2; -- أول فهرسين
-- النتائج:
-- Ali
-- Alaa
SELECT * FROM names_table LIMIT 2, 4; -- من الفهرس 2 إلى الفهرس 4
-- النتائج:
-- Ahmed
-- Ola
-- Mohamed
-- Mahmoud
```

##### OFFSETs - الإزاحات

- *البحث بعد إزاحة معينة*

```sql
SELECT * FROM names_table LIMIT 3 OFFSET 2;  
-- Ahmed
-- Ola
-- Mohamed
```

##### ORDER BY - الطلب حسب

- *البحث حسب ترتيب معين*
- *الحقل النصي الترتيب من خلاله يكون أبجديا*
- `ASC`: الترتيب الافتراضي (الترتيب تصاعديا)
- `DESC`: عكس الترتيب (الترتيب تنازليا)

```sql
SELECT * FROM names_table ORDER BY name;
-- Or
SELECT * FROM names_table ORDER BY name ASC;
-- النتائج:
-- Ahmed
-- Alaa
-- Ali
-- Mahmoud
-- Mohamed
-- Ola
SELECT * FROM names_table ORDER BY name DESC;
-- النتائج:
-- Ola
-- Mohamed
-- Mahmoud
-- Ali
-- Alaa
-- Ahmed

SELECT * FROM names_table ORDER BY name LIMIT 4 OFFSET 2;
-- Ali
-- Mahmoud
-- Mohamed
-- Ola

-- SQL Server
-- الفهرس يبدأمن 0
SELECT * FROM names_table ORDER BY name OFFSET 1 ROWS FETCH NEXT 3 ROWS ONLY;
```

--

#### Indexes - الفهارس

الفهرس هو بنية بيانات خاصة تُستخدم لتسريع عمليات استرجاع البيانات من الجداول. يعمل مثل "فهرس الكتاب" الذي يساعدك على العثور على المعلومات بسرعة بدلاً من البحث في كل الصفحات.

--

**أنواع الفهارس:**

1. الفهرس العادي (`INDEX`):

    ```sql
    -- إنشاء فهرس على عمود واحد
    CREATE INDEX idx_email ON users(email);

    -- إنشاء فهرس على عدة أعمدة
    CREATE INDEX idx_name_age ON users(first_name, last_name, age);
    ```

2. الفهرس الفريد (`UNIQUE INDEX`):

    ```sql
    -- يمنع تكرار القيم
    CREATE UNIQUE INDEX idx_unique_email ON users(email);
    ```

3. الفهرس النصي (`FULLTEXT INDEX`)

    ```sql
    -- للبحث النصي
    CREATE FULLTEXT INDEX idx_content ON articles(content);
    ```

4. الفهرس المكاني (`SPATIAL INDEX`)

    ```sql
    -- للبيانات الجغرافية
    CREATE SPATIAL INDEX idx_location ON maps(coordinates);
    ```

**كيف يعمل الفهرس؟:**

- *بدون فهرس:*

```sql
-- مسح كامل للجدول (Full Table Scan)
SELECT * FROM users WHERE email = 'ahmed@example.com';
```

- *بفهرس:*

```sql
-- بحث سريع باستخدام شجرة B-tree
SELECT * FROM users WHERE email = 'ahmed@example.com';
```

**أمثلة عملية:**

*إنشاء فهارس مع الجداول:*

```sql
CREATE TABLE employees (
    id INT PRIMARY KEY,                    -- PRIMARY KEY ينشئ فهرس تلقائي
    email VARCHAR(100) UNIQUE,            -- UNIQUE ينشئ فهرس تلقائي
    first_name VARCHAR(50),
    last_name VARCHAR(50),
    salary DECIMAL(10,2),
    hire_date DATE,
    
    -- إنشاء فهارس إضافية
    INDEX idx_name (first_name, last_name),
    INDEX idx_salary (salary),
    INDEX idx_hire_date (hire_date)
);
```

*إدارة الفهارس:*

```sql
-- عرض الفهارس
SHOW INDEX FROM employees;

-- إضافة فهرس لجدول موجود
CREATE INDEX idx_department ON employees(department_id);

-- حذف فهرس
DROP INDEX idx_department ON employees;
```

**متى نستخدم الفهارس؟:**

- الأعمدة المستخدمة في `WHERE`
- الأعمدة المستخدمة في `JOIN`
- الأعمدة المستخدمة في `ORDER BY`
- الأعمدة ذات القيم الفريدة أو شبه الفريدة
- الجداول الكبيرة (أكثر من 10,000 صف)

**❌ حالات غير مناسبة:**

- الجداول الصغيرة
- الأعمدة التي نادراً ما تُستخدم في البحث
- الأعمدة التي تحتوي على قيم متكررة كثيرة
- جداول يتم الكتابة فيها أكثر من القراءة

**تأثير الفهارس على الأداء:**

- *المزايا:*
  - ⚡ تسريع استعلامات البحث
  - 🚀 تحسين أداء `JOIN` و `ORDER BY`
  - 📈 كفاءة أفضل للاستعلامات المعقدة

- *العيوب:*
  - 💾 مساحة تخزين إضافية
  - ⏱️ إبطاء عمليات `INSERT`/`UPDATE`/`DELETE`
  - 🛠️ صيانة إضافية للفهارس

**أمثلة عملية على استخدام الفهارس:**

- *استعلام بدون فهرس:*

```sql
-- بطيء على جداول كبيرة
SELECT * FROM orders 
WHERE customer_id = 100 
AND order_date BETWEEN '2024-01-01' AND '2024-12-31';
```

- *استعلام بفهرس:*

```sql
-- سريع بعد إنشاء الفهرس
CREATE INDEX idx_customer_date ON orders(customer_id, order_date);

SELECT * FROM orders 
WHERE customer_id = 100 
AND order_date BETWEEN '2024-01-01' AND '2024-12-31';
```

**نصائح مهمة:**

*استراتيجيات الفهرسة:*

1. **فهرس المركبة (Composite Index):**

   ```sql
   -- أفضل من فهارس منفصلة
   CREATE INDEX idx_name_department ON employees(first_name, department_id);
   ```

2. **اختيار ترتيب الأعمدة:**

   ```sql
   -- ضع الأعمدة الأكثر انتقائية أولاً
   CREATE INDEX idx_department_name ON employees(department_id, first_name);
   ```

3. **مراقبة أداء الفهارس:**

   ```sql
   -- استخدام EXPLAIN لتحليل الاستعلامات
   EXPLAIN SELECT * FROM employees WHERE first_name = 'Ahmed';
   ```

--

#### Built-in Functions - الدوال المدمجة

- المرجع الخاص بدوال `MySQL` الإصدار التاسع: [Built-In Function and Operator Reference](https://dev.mysql.com/doc/refman/9.5/en/built-in-function-reference.html)

- `COS`: جيب التمام
- `PI`: باي (22/7)

```sql
SELECT COS(PI()); -- (-1)
```

- `CONCAT`: ربط البيانات

```sql
SELECT CONCAT(1, 2);
-- النتائج
-- CONCAT(1, 2)
-- 12

SELECT CONCAT('A', 'l', 'i') AS name; -- AS: تغير اسم العمود
-- النتائج
-- name
-- Ali

CREATE TABLE users(f_name VARCHAR(50), l_name VARCHAR(50));
INSERT INTO users VALUES
('Hazim', 'Nabil'),
('Hamza', 'Ramadan'),
('Sameer', 'Badr'),
('Emad', 'Emam');
SELECT CONCAT(f_name, l_name) AS 'Fullname' FROM users;
-- النتائج
-- HazimNabil
-- HamzaRamadan
-- SameerBadr
-- EmadEmam
SELECT CONCAT(f_name, ' ', l_name) AS 'Fullname' FROM users;
-- النتائج
-- Hazim Nabil
-- Hamza Ramadan
-- Sameer Badr
-- Emad Emam
```

- `CONCAT_WS`: ربط البيانات بعامل محدد

```sql
SELECT CONCAT_WS(' ', f_name, l_name) AS 'Fullname' FROM users;
-- النتائج
-- Hazim Nabil
-- Hamza Ramadan
-- Sameer Badr
-- Emad Emam

SELECT CONCAT_WS('-', f_name, l_name) AS 'Fullname' FROM users;
-- النتائج
-- Hazim-Nabil
-- Hamza-Ramadan
-- Sameer-Badr
-- Emad-Emam
```

- `SUBSTR`: تحديد جزء من النص

```SQL
SELECT SUBSTR(f_name, 2) FROM users;
-- النتائج
-- azim
-- amza
-- ameer
-- mad
SELECT SUBSTR(f_name, 1 ,3) FROM users;
-- النتائج
-- Haz
-- Ham
-- Sam
-- Ema
```

- `LEFT`: تحديد جزء من يسار النص

```SQL
SELECT LEFT(f_name, 3) FROM users;
-- النتائج
-- Haz
-- Ham
-- Sam
-- Ema
```

- `RIGHT`: تحديد جزء من يمين النص

```SQL
SELECT RIGHT(f_name, 3) FROM users;
-- النتائج
-- zim
-- mza
-- eer
-- mad
```

- `LENGTH`: تحديد طول النص

```SQL
SELECT SUBSTR(f_name, 2) FROM users;
-- النتائج
-- 5
-- 5
-- 6
-- 4
```

- `COUNT`: عدد الصفوف التي لها قيم (`NOT NULL`)

```sql
SELECT COUNT(f_name) FROM users;
-- أو تحديد كل الأعمدة:
SELECT COUNT(*) FROM users;
-- النتائج
-- 4
```

- `MIN`, `MAX`: أصغر وأكبر قيمة
  - لو القيمة نصية يعتمد على ترتيب اول حرف

```sql
SELECT MIN(f_name) FROM users;
-- Emad
SELECT MAX(f_name) FROM users;
-- Sameer
```

- `AVG`: الوسط الحسابي
  - يجب أن تكون البيانات رقمية

```sql
CREATE TABLE numbers(number INT);
INSERT INTO numbers VALUES(10), (50), (100), (200), (300);
SELECT AVG(number) FROM numbers; -- 132.0000
```

- `ROUND`: أقرب علامة عشرية

```sql
SELECT ROUND(number, 2) FROM numbers;
```

- `DISTINCT`: تصفية البيانات المكررة

```sql
CREATE TABLE letters(letter VARCHAR(1));
INSERT INTO letters VALUES('A'), ('B'), ('A'), ('C');
SELECT DISTINCT(letter) FROM letters; -- A B C
```

--

- أهم `Built-in Functions`

##### 🔢 **الدوال الرياضية (Mathematical Functions)**

```sql
-- الأساسية
SELECT ABS(-10);        -- 10 (قيمة مطلقة)
SELECT ROUND(15.75);    -- 16 (تقريب)
SELECT CEIL(15.2);      -- 16 (تقريب لأعلى)
SELECT FLOOR(15.8);     -- 15 (تقريب لأسفل)
SELECT POW(2, 3);       -- 8 (أس)
SELECT SQRT(16);        -- 4 (جذر تربيعي)

-- العشوائية
SELECT RAND();          -- رقم عشوائي بين 0 و 1
SELECT FLOOR(RAND() * 100); -- رقم عشوائي بين 0 و 99
```

##### 📊 **دوال التجميع (Aggregate Functions)**

```sql
-- الأساسية
SELECT COUNT(*) FROM users;                    -- عدد الصفوف
SELECT AVG(salary) FROM employees;            -- متوسط
SELECT SUM(amount) FROM orders;               -- مجموع
SELECT MAX(price) FROM products;              -- أعلى قيمة
SELECT MIN(age) FROM customers;               -- أقل قيمة

-- متقدمة
SELECT GROUP_CONCAT(name) FROM users;         -- دمج قيم نصية
SELECT COUNT(DISTINCT department) FROM employees; -- قيم فريدة
```

##### 📅 **دوال التاريخ والوقت (Date & Time Functions)**

```sql
-- التاريخ والوقت الحالي
SELECT NOW();           -- 2024-01-15 10:30:25
SELECT CURDATE();       -- 2024-01-15
SELECT CURTIME();       -- 10:30:25

-- استخراج أجزاء من التاريخ
SELECT YEAR(NOW());     -- 2024
SELECT MONTH(NOW());    -- 1
SELECT DAY(NOW());      -- 15
SELECT HOUR(NOW());     -- 10
SELECT MINUTE(NOW());   -- 30

-- العمليات على التاريخ
SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);    -- إضافة 7 أيام
SELECT DATE_SUB(NOW(), INTERVAL 1 MONTH);  -- طرح شهر
SELECT DATEDIFF('2024-01-20', '2024-01-15'); -- فرق الأيام: 5

-- التنسيق
SELECT DATE_FORMAT(NOW(), '%Y-%m-%d');     -- 2024-01-15
SELECT DATE_FORMAT(NOW(), '%W, %M %Y');    -- Monday, January 2024
```

##### 📝 **الدوال النصية (String Functions)**

```sql
-- التحويل والحالة
SELECT UPPER('hello');        -- HELLO
SELECT LOWER('HELLO');        -- hello
SELECT CONCAT('Hello', ' ', 'World'); -- Hello World

-- الاستخراج والبحث
SELECT SUBSTRING('Hello World', 1, 5); -- Hello
SELECT LENGTH('Hello');                -- 5
SELECT LOCATE('World', 'Hello World'); -- 7 (الموقع)

-- التعديل
SELECT TRIM('  Hello  ');              -- Hello
SELECT REPLACE('Hello World', 'World', 'MySQL'); -- Hello MySQL
SELECT REVERSE('Hello');               -- olleH

-- التقسيم والدمج
SELECT CONCAT_WS(', ', 'John', 'Doe'); -- John, Doe
SELECT SUBSTRING_INDEX('www.example.com', '.', 2); -- www.example
```

##### 🔍 **دوال الشرطية (Conditional Functions)**

```sql
-- إنشاء جدول employees
CREATE TABLE employees (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100) NOT NULL,
    salary DECIMAL(10,2) NOT NULL,
    department VARCHAR(50),
    hire_date DATE
);

-- إدراج البيانات
INSERT INTO employees (name, salary, department, hire_date) VALUES
('أحمد محمد', 7500.00, 'التطوير', '2020-03-15'),
('فاطمة علي', 4500.00, 'التسويق', '2021-06-20'),
('يوسف خالد', 6000.00, 'المبيعات', '2019-11-10'),
('ليلى عبدالله', 5500.00, 'التطوير', '2022-01-05'),
('محمد حسن', 8000.00, 'الإدارة', '2018-08-12'),
('سارة ناصر', 4800.00, 'التسويق', '2023-02-28'),
('خالد إبراهيم', 3000.00, 'الدعم الفني', '2022-09-15');
```

```sql
-- عرض جميع الموظفين
SELECT * FROM employees;
```

**النتيجة:**

```text
+----+----------------+---------+-------------+------------+
| id | name           | salary  | department  | hire_date  |
+----+----------------+---------+-------------+------------+
|  1 | أحمد محمد     | 7500.00 | التطوير    | 2020-03-15 |
|  2 | فاطمة علي      | 4500.00 | التسويق    | 2021-06-20 |
|  3 | يوسف خالد      | 6000.00 | المبيعات   | 2019-11-10 |
|  4 | ليلى عبدالله  | 5500.00 | التطوير    | 2022-01-05 |
|  5 | محمد حسن      | 8000.00 | الإدارة    | 2018-08-12 |
|  6 | سارة ناصر      | 4800.00 | التسويق    | 2023-02-28 |
|  7 | خالد إبراهيم   | 3000.00 | الدعم الفني | 2022-09-15 |
+----+----------------+---------+-------------+------------+
```

```sql
-- استخدام IF لتصنيف الرواتب
SELECT 
    name,
    salary,
    IF(salary > 5000, 'High', 'Low') as salary_category
FROM employees;
```

**النتيجة:**

+----------------+---------+-----------------+
| name           | salary  | salary_category |
+----------------+---------+-----------------+
| أحمد محمد     | 7500.00 | High            |
| فاطمة علي      | 4500.00 | Low             |
| يوسف خالد      | 6000.00 | High            |
| ليلى عبدالله  | 5500.00 | High            |
| محمد حسن      | 8000.00 | High            |
| سارة ناصر      | 4800.00 | Low             |
| خالد إبراهيم   | 3000.00 | Low             |
+----------------+---------+-----------------+

```sql
-- استخدام CASE لتصنيف المستويات الوظيفية
SELECT 
    name,
    salary,
    department,
    CASE 
        WHEN salary > 7000 THEN 'Manager'
        WHEN salary > 5000 THEN 'Senior'
        ELSE 'Junior'
    END as level
FROM employees
ORDER BY salary DESC;
```

**النتيجة:**

+----------------+---------+-------------+--------+
| name           | salary  | department  | level  |
+----------------+---------+-------------+--------+
| محمد حسن      | 8000.00 | الإدارة     | Manager|
| أحمد محمد     | 7500.00 | التطوير     | Manager|
| يوسف خالد      | 6000.00 | المبيعات    | Senior |
| ليلى عبدالله  | 5500.00 | التطوير     | Senior |
| سارة ناصر      | 4800.00 | التسويق     | Junior |
| فاطمة علي      | 4500.00 | التسويق     | Junior |
| خالد إبراهيم   | 3000.00 | الدعم الفني | Junior |
+----------------+---------+-------------+--------+

```sql
-- إحصائيات حسب المستوى
SELECT 
    CASE 
        WHEN salary > 7000 THEN 'Manager'
        WHEN salary > 5000 THEN 'Senior'
        ELSE 'Junior'
    END as level,
    COUNT(*) as employee_count,
    ROUND(AVG(salary), 2) as avg_salary,
    MIN(salary) as min_salary,
    MAX(salary) as max_salary
FROM employees
GROUP BY level
ORDER BY avg_salary DESC;
```

**النتيجة:**

+--------+----------------+------------+------------+------------+
| level  | employee_count | avg_salary | min_salary | max_salary |
+--------+----------------+------------+------------+------------+
| Manager|              2 |    7750.00 |    7500.00 |    8000.00 |
| Senior |              2 |    5750.00 |    5500.00 |    6000.00 |
| Junior |              3 |    4100.00 |    3000.00 |    4800.00 |
+--------+----------------+------------+------------+------------+

- ملاحظات مهمة:

1. **دالة IF**: تستخدم للشروط البسيطة ذات نتيجتين فقط
2. **دالة CASE**: أكثر مرونة للشروط المتعددة والقيم المعقدة
3. **الترتيب**: CASE يتم تقييم الشروط بالترتيب (من الأعلى للأسفل)
4. **الأداء**: كلتا الدالتين فعالة في معالجة البيانات على مستوى قاعدة البيانات

```sql
-- COALESCE (أول قيمة غير NULL)
SELECT COALESCE(NULL, NULL, 'Hello', 'World'); -- Hello

-- NULLIF (يعيد NULL إذا تساوى المدخلان)
SELECT NULLIF(10, 10); -- NULL
SELECT NULLIF(10, 5);  -- 10
```

##### 🛡️ **دوال الأمان (Security Functions)**

```sql
-- التشفير
SELECT MD5('password');        -- تشفير MD5
SELECT SHA1('password');       -- تشفير SHA1
SELECT SHA2('password', 256);  -- تشفير SHA256

-- الأساسية
SELECT PASSWORD('mypass');     -- تشفير كلمة المرور (مهمل في الإصدارات الحديثة)
```

- التفصيل:

```sql
-- هذه دوال تشفير (Hash Functions) تحول النص إلى قيمة مشفرة ثابتة الطول
SELECT MD5('password');        -- produces: 5f4dcc3b5aa765d61d8327deb882cf99
SELECT SHA1('password');       -- produces: 5baa61e4c9b93f3f0682250b6cf8331b7ee68fd8
SELECT SHA2('password', 256);  -- produces: 5e884898da28047151d0e56f8dc6292773603d0d6aabbdd62a11ef721d1542d8
```

- مثال عملي:

```sql
-- إنشاء جدول مستخدمين مع كلمات مرور مشفرة
CREATE TABLE users (
    id INT PRIMARY KEY AUTO_INCREMENT,
    username VARCHAR(50),
    password_hash VARCHAR(64)  -- لتخزين SHA256
);

-- إدراج مستخدم بكلمة مرور مشفرة
INSERT INTO users (username, password_hash) 
VALUES ('ahmed', SHA2('mysecret123', 256));

-- التحقق من كلمة المرور عند تسجيل الدخول
SELECT * FROM users 
WHERE username = 'ahmed' 
AND password_hash = SHA2('mysecret123', 256);
```

##### 📋 **الدوال الخاصة بـ JSON**

```sql
-- إنشاء وتحليل JSON
-- JSON_OBJECT: إنشاء كائن JSON من أزواج مفتاح-قيمة
SELECT JSON_OBJECT('name', 'John', 'age', 30, 'city', 'Cairo');
-- النتيجة: {"name": "John", "age": 30, "city": "Cairo"}

-- JSON_EXTRACT: استخراج قيمة من كائن JSON
SELECT JSON_EXTRACT('{"name": "John", "age": 30}', '$.name');
-- النتيجة: "John"

-- البحث في JSON
SELECT * FROM users WHERE JSON_CONTAINS(metadata, '{"status": "active"}');
```

- مثال عملي مع جدول:

```sql
-- إنشاء جدول مع عمود JSON
CREATE TABLE products (
    id INT PRIMARY KEY,
    name VARCHAR(100),
    metadata JSON
);

-- إدراج بيانات JSON
INSERT INTO products VALUES 
(1, 'Laptop', '{"brand": "Dell", "specs": {"ram": "16GB", "storage": "512GB"}, "price": 1500}'),
(2, 'Phone', '{"brand": "Samsung", "specs": {"ram": "8GB", "storage": "128GB"}, "price": 800}');

-- البحث في بيانات JSON
SELECT * FROM products 
WHERE JSON_EXTRACT(metadata, '$.price') > 1000;

-- أو باستخدام JSON_CONTAINS
SELECT * FROM products 
WHERE JSON_CONTAINS(metadata, '"Dell"', '$.brand');
```

- `JSON_CONTAINS` بالتفصيل:

```sql
-- إنشاء جدول المستخدمين مع metadata كـ JSON
CREATE TABLE users (
    id INT PRIMARY KEY,
    name VARCHAR(100),
    metadata JSON
);

-- إدراج بيانات
INSERT INTO users VALUES 
(1, 'Ahmed', '{"status": "active", "preferences": {"theme": "dark", "language": "ar"}}'),
(2, 'Fatima', '{"status": "inactive", "preferences": {"theme": "light", "language": "en"}}'),
(3, 'Youssef', '{"status": "active", "preferences": {"theme": "dark", "language": "fr"}}');

-- البحث عن المستخدمين النشطين
SELECT * FROM users 
WHERE JSON_CONTAINS(metadata, '{"status": "active"}');
-- سيعيد: Ahmed و Youssef فقط

-- البحث في nested objects
SELECT * FROM users 
WHERE JSON_CONTAINS(metadata, '"dark"', '$.preferences.theme');
```

##### 🎯 **دوال التحقق من NULL**

```sql
SELECT ISNULL(NULL);        -- 1 (TRUE)
SELECT ISNULL('Hello');     -- 0 (FALSE)

SELECT IFNULL(NULL, 'Default Value'); -- Default Value
```

##### 💾 **دوال لنظام وإدارة البيانات**

```sql
-- معلومات الاتصال
SELECT CONNECTION_ID();     -- معرف الاتصال الحالي
SELECT DATABASE();          -- اسم قاعدة البيانات الحالية
SELECT USER();              -- المستخدم الحالي
SELECT VERSION();           -- إصدار MySQL

-- التحكم في التكرار
SELECT UUID();              -- إنشاء معرف فريد عالمي
```

- `CONNECTION_ID()`:

```sql
-- يعيد معرف فريد للاتصال الحالي بقاعدة البيانات
SELECT CONNECTION_ID();
-- النتيجة: 45 (رقم مختلف لكل اتصال)

-- هذا مفيد للتتبع والتصحيح
SELECT CONNECTION_ID() as connection_id, 
       USER() as currentUser, 
       DATABASE() as current_database;
```

- `UUID()` - المعرف الفريد العالمي:

```sql
-- إنشاء معرف فريد عالمي (مثل: 550e8400-e29b-41d4-a716-446655440000)
SELECT UUID();
-- النتيجة: 6ccd780c-baba-1026-9564-0040f4311e29 (قيمة مختلفة في كل مرة)

-- استخدام عملي في الجداول
CREATE TABLE orders (
    id VARCHAR(36) PRIMARY KEY,
    customer_name VARCHAR(100),
    amount DECIMAL(10,2)
);

-- إدراج طلب بدون تحديد ID (سيتم توليده تلقائياً)
INSERT INTO orders (id, customer_name, amount) 
VALUES (UUID(), 'Mohamed Ali', 150.00);

-- عرض البيانات
SELECT * FROM orders;
-- النتيجة: 
-- id: 6ccd780c-baba-1026-9564-0040f4311e29, customer_name: Mohamed Ali, amount: 150.00
```

- مثال متكامل عملي:

```sql
-- نظام مستخدمين متكامل مع UUID وتشفير
CREATE TABLE system_users (
    id VARCHAR(36) PRIMARY KEY,
    username VARCHAR(50) UNIQUE,
    email VARCHAR(100),
    password_hash VARCHAR(64),
    profile_data JSON,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-- إدراج مستخدم جديد
INSERT INTO system_users (username, email, password_hash, profile_data) 
VALUES (
    UUID(),
    'ali_tech',
    'ali@example.com',
    SHA2('SecurePass123!', 256),
    JSON_OBJECT(
        'full_name', 'Ali Technology',
        'role', 'admin',
        'settings', JSON_OBJECT('notifications', true, 'theme', 'dark')
    )
);

-- البحث في النظام
SELECT 
    id,
    username,
    JSON_EXTRACT(profile_data, '$.full_name') as full_name,
    JSON_EXTRACT(profile_data, '$.role') as role,
    CONNECTION_ID() as query_connection_id
FROM system_users 
WHERE JSON_CONTAINS(profile_data, '"admin"', '$.role');
```

##### 🚀 **أمثلة عملية للاستخدام في التطبيقات**

- مثال 1: إدارة المستخدمين

```sql
-- إنشاء جدول users
CREATE TABLE users (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100) NOT NULL,
    email VARCHAR(150) NOT NULL,
    password VARCHAR(255) NOT NULL,
    birth_date DATE,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-- إدراج بيانات المستخدمين
INSERT INTO users (name, email, password, birth_date) VALUES
('أحمد خالد', '  AHMED@Example.Com  ', 'pass123', '1990-05-15'),
('فاطمة محمد', 'fatima.test@domain.com', 'strongpassword123', '1985-12-20'),
('يوسف علي', '  YOUSEF@test.COM  ', 'weak', '1995-08-30'),
('ليلى حسن', 'leila.hassan@email.com', 'securepass456', '1988-03-10'),
('محمد إبراهيم', 'MOHAMMED@DOMAIN.COM  ', 'short', '1992-11-25'),
('سارة ناصر', 'sara.nasser@example.com', 'verylongpassword789', '1998-07-03');

-- التحقق من البريد الإلكتروني
SELECT 
    id,
    name,
    email as original_email,
    LOWER(TRIM(email)) as clean_email,
    CASE 
        WHEN LENGTH(password) >= 8 THEN 'Strong'
        ELSE 'Weak'
    END as password_strength,
    LENGTH(password) as password_length
FROM users;

-- حساب عمر المستخدم
SELECT 
    name,
    birth_date,
    TIMESTAMPDIFF(YEAR, birth_date, CURDATE()) as age
FROM users
ORDER BY age DESC;
```

- مثال 2: التقارير والإحصائيات

```sql
-- إنشاء جدول orders
CREATE TABLE orders (
    order_id INT PRIMARY KEY AUTO_INCREMENT,
    customer_id INT,
    amount DECIMAL(10,2) NOT NULL,
    order_date DATETIME NOT NULL,
    status VARCHAR(20) DEFAULT 'completed'
);

-- إدراج بيانات الطلبات
INSERT INTO orders (customer_id, amount, order_date) VALUES
(1, 150.00, '2024-01-15 10:30:00'),
(2, 75.50, '2024-01-20 14:22:00'),
(3, 200.00, '2024-02-05 09:15:00'),
(1, 89.99, '2024-02-10 16:45:00'),
(4, 300.25, '2024-02-28 11:20:00'),
(2, 45.00, '2024-03-02 13:10:00'),
(5, 120.75, '2024-03-02 15:30:00'),
(3, 180.00, '2024-03-15 08:45:00'),
(1, 95.60, '2024-03-20 12:00:00'),
(6, 250.00, '2024-03-25 17:20:00');

-- تقرير المبيعات الشهري
SELECT 
    DATE_FORMAT(order_date, '%Y-%m') as month,
    COUNT(*) as total_orders,
    SUM(amount) as total_revenue,
    ROUND(AVG(amount), 2) as avg_order_value,
    MIN(amount) as min_order,
    MAX(amount) as max_order
FROM orders
GROUP BY DATE_FORMAT(order_date, '%Y-%m')
ORDER BY month;
```

- مثال 3: معالجة البيانات

```sql
-- إنشاء جدول products
CREATE TABLE products (
    product_id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(200) NOT NULL,
    description TEXT,
    price DECIMAL(10,2),
    category VARCHAR(50)
);

-- إدراج بيانات المنتجات
INSERT INTO products (name, description, price, category) VALUES
('لابتوب ديل', '   هذا لابتوب قوي جدا مع معالج i7 وذاكرة 16GB ومساحة تخزين 512GB SSD وشاشة 15 بوصة. مناسب للأعمال والدراسة   ', 2500.00, 'إلكترونيات'),
('هاتف سامسونج', 'هاتف ذكي بشاشة 6.7 بوصة وكاميرا 108 ميجابكسل وبطارية 5000 مللي أمبير. يدعم 5G ويأتي مع قلم S-Pen.', 1200.00, 'هواتف'),
('كتاب البرمجة', '   كتاب شامل لتعليم لغة Python للمبتدئين مع أمثلة عملية ومشاريع تطبيقية. يحتوي على 300 صفحة ملونة.   ', 45.00, 'كتب'),
('سماعات رأس', 'سماعات لاسلكية مع إلغاء الضوضاء النشط ومدة بطارية تصل إلى 30 ساعة. جودة صوت عالية وتصميم مريح.', 300.00, 'إلكترونيات'),
('حقيبة ظهر', '   حقيبة ظهر كبيرة الحجم مضادة للماء تحتوي على多个 الجيوب ومناسبة للجامعة والسفر. مصنوعة من مواد متينة.   ', 80.00, 'أكسسوارات');

-- عرض البيانات الأصلية
SELECT 
    product_id,
    name as original_name,
    LENGTH(description) as desc_length,
    description as original_description
FROM products;

-- تنظيف وتنسيق البيانات
UPDATE products 
SET 
    name = TRIM(name),
    description = CONCAT(SUBSTRING(description, 1, 100), '...')
WHERE LENGTH(description) > 100;

-- عرض البيانات بعد المعالجة
SELECT 
    product_id,
    name as cleaned_name,
    LENGTH(description) as new_desc_length,
    description as new_description
FROM products;
```

- ⚡ نصائح للأداء

1. **استخدم الفهرس مع الدوال بحذر**
2. **تجنب الدوال على الأعمدة في WHERE**
3. **استخدم الدوال المدمجة بدلاً من معالجة البيانات في التطبيق**

--

#### VIEW - العرض

**الـ View** هي جدول افتراضي (`Virtual Table`) يتم إنشاؤها بناءً على نتيجة استعلام `SQL`. تعتبر "نافذة" على البيانات الحقيقية في الجداول.

- إنشاء `View`:

```sql
CREATE VIEW view_name AS
SELECT column1, column2, ...
FROM table_name
WHERE condition;
```

- مثال عملي:

```sql
-- إنشاء جدول كمثال
CREATE TABLE employees (
    id INT PRIMARY KEY,
    name VARCHAR(100),
    department VARCHAR(50),
    salary DECIMAL(10,2),
    hire_date DATE
);

-- إدراج بيانات
INSERT INTO employees VALUES
(1, 'أحمد', 'المبيعات', 5000, '2020-01-15'),
(2, 'محمد', 'التسويق', 6000, '2019-03-20'),
(3, 'فاطمة', 'المبيعات', 5500, '2021-06-10'),
(4, 'ليلى', 'التطوير', 7000, '2018-11-05');

-- إنشاء view
CREATE VIEW sales_employees AS
SELECT id, name, salary, hire_date
FROM employees
WHERE department = 'المبيعات';
```

- استخدام الـ `View`:

```sql
-- الاستعلام من الـ View كأي جدول عادي
SELECT * FROM sales_employees;

-- يمكن إضافة شروط
SELECT * FROM sales_employees WHERE salary > 5200;

-- استخدام مع JOIN
CREATE VIEW employee_details AS
SELECT e.name, e.department, e.salary, d.manager
FROM employees e
JOIN departments d ON e.department = d.dept_name;
```

- تحديث `View`:

```sql
-- تحديث View موجود
CREATE OR REPLACE VIEW sales_employees AS
SELECT id, name, salary, hire_date, department
FROM employees
WHERE department = 'المبيعات'
AND salary > 4500;
```

- أنواع الـ `Views`:

1. **View بسيطة (Simple View)**

    ```sql
    CREATE VIEW high_salary_employees AS
    SELECT name, department, salary
    FROM employees
    WHERE salary > 6000;
    ```

2. **View معقدة (Complex View)**

```sql
CREATE VIEW department_summary AS
SELECT 
    department,
    COUNT(*) as employee_count,
    AVG(salary) as avg_salary,
    MAX(salary) as max_salary
FROM employees
GROUP BY department;
```

- تحديث البيانات عبر `View`:

**يمكن تحديث البيانات عبر View بشروط:**

```sql
-- View قابل للتحديث
CREATE VIEW updatable_employees AS
SELECT id, name, department
FROM employees;

-- تحديث البيانات
UPDATE updatable_employees 
SET department = 'التسويق' 
WHERE id = 1;
```

- حذف `View`:

```sql
DROP VIEW view_name;

-- مثال
DROP VIEW sales_employees;
```

- عرض معلومات الـ `Views`:

```sql
-- عرض جميع الـ Views
SHOW FULL TABLES WHERE TABLE_TYPE LIKE 'VIEW';

-- عرض تعريف View
SHOW CREATE VIEW view_name;
```

- فوائد استخدام الـ `Views`:

1. **الأمان**

    ```sql
    -- منح صلاحية الوصول للـ View فقط وليس الجداول الأصلية
    CREATE VIEW public_employee_info AS
    SELECT name, department
    FROM employees;

    -- عرض المستخدمين الموجودين
    SELECT user, host FROM mysql.user;

    -- إنشاء مستخدم
    CREATE USER 'new_user'@'localhost' IDENTIFIED BY 'strong_password';

    -- منح الصلاحية لمستخدم موجود
    GRANT SELECT ON public_employee_info TO 'user'@'host';

    -- منح الصلاحية للمستخدم الحالي
    GRANT SELECT ON public_employee_info TO CURRENT_USER();

    -- تأكيد الصلاحيات الممنوحة
    SHOW GRANTS FOR 'user'@'host';
    -- عرض صلاحياتك الحالية
    SHOW GRANTS;

    -- التحقق إذا كان لديك صلاحية CREATE USER
    SELECT * FROM mysql.user WHERE user = CURRENT_USER();
    ```

2. **تبسيط الاستعلامات المعقدة**

    ```sql
    -- بدلاً من كتابة استعلام معقد كل مرة
    CREATE VIEW monthly_sales_report AS
    SELECT 
        YEAR(sale_date) as year,
        MONTH(sale_date) as month,
        product_id,
        SUM(amount) as total_sales,
        COUNT(*) as transaction_count
    FROM sales
    GROUP BY YEAR(sale_date), MONTH(sale_date), product_id;
    ```

3. **الاتساق المنطقي**

    ```sql
    CREATE VIEW active_customers AS
    SELECT customer_id, name, email
    FROM customers
    WHERE status = 'active'
    AND last_purchase_date > DATE_SUB(NOW(), INTERVAL 6 MONTH);
    ```

- قيود الـ `Views`:

  - بعض الـ `Views` غير قابلة للتحديث
  - قد تؤثر على الأداء إذا كانت معقدة جداً
  - لا يمكن إنشاء فهارس على الـ `Views` (في معظم حالات `MySQL`)

- مثال متكامل:

```sql
-- إنشاء View متقدم
CREATE VIEW employee_performance AS
SELECT 
    e.id,
    e.name,
    e.department,
    e.salary,
    COUNT(p.project_id) as project_count,
    AVG(p.rating) as avg_rating
FROM employees e
LEFT JOIN projects p ON e.id = p.employee_id
GROUP BY e.id, e.name, e.department, e.salary;

-- استخدام الـ View
SELECT * FROM employee_performance 
WHERE avg_rating > 4.0 
ORDER BY salary DESC;
```

--

#### Prepared Statements - البيانات المعدة

(البيانات المعدة مسبقاً) هي طريقة أمنة لتنفيذ استعلامات `SQL` عن طريق فصل البيانات عن الشفرة (`code`).

- *المشكلة التي تحلها:*

```sql
-- ❌ الطريقة الخطرة (SQL Injection)
"SELECT * FROM users WHERE email = '" + user_input + "'"

-- إذا كان user_input = "' OR '1'='1"
-- يصبح الاستعلام: SELECT * FROM users WHERE email = '' OR '1'='1'
-- وهذا سيعيد جميع المستخدمين!
```

- *الحل مع Prepared Statements:*

```sql
-- ✅ الطريقة الآمنة
"SELECT * FROM users WHERE email = ?"
-- ثم نربط القيمة لاحقاً
```

- *مزايا Prepared Statements*

- 🛡️ *منع هجمات SQL Injection*
- 🚀 *أداء أفضل* (خاصة مع التكرار)
- 📝 *كود أكثر نظافة وأماناً*
- 🔄 *إعادة استخدام خطط التنفيذ*

--

- *أنواع Prepared Statements في MySQL*

- في `SQL` مباشرة:

```sql
-- إعداد الاستعلام
PREPARE user_stmt FROM 'SELECT * FROM users WHERE id = ?';

-- تنفيذ مع قيم
SET @user_id = 1;
EXECUTE user_stmt USING @user_id;

-- تنظيف
DEALLOCATE PREPARE user_stmt;
```

- في لغات البرمجة (مثل `Python`) - الأهم

--

#### Subquery - الاستعلام الفرعي

**الـ Subquery** (الاستعلام الفرعي) هو استعلام داخل استعلام آخر. يُستخدم لتنفيذ عمليات معقدة حيث تحتاج نتيجة استعلام كمدخل لاستعلام آخر.

- مثال: تمكن `Subquery` من استخدام دوال التجميع (AVG, SUM, COUNT, MAX, MIN) بشكل صحيح في جملة `WHERE`.

- 📝 **البناء الأساسي**

```sql
SELECT column1, column2
FROM table1
WHERE column1 = (SELECT column1 FROM table2 WHERE condition);
```

- 🏢 **إنشاء الجداول للتمارين**

```sql
-- جدول الموظفين
CREATE TABLE employees (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100),
    department VARCHAR(50),
    salary DECIMAL(10,2),
    hire_date DATE
);

-- جدول الأقسام
CREATE TABLE departments (
    dept_id INT PRIMARY KEY,
    dept_name VARCHAR(50),
    manager_id INT,
    budget DECIMAL(12,2)
);

-- جدول المشاريع
CREATE TABLE projects (
    project_id INT PRIMARY KEY,
    project_name VARCHAR(100),
    department VARCHAR(50),
    budget DECIMAL(10,2),
    start_date DATE
);

-- إدراج البيانات
INSERT INTO employees (name, department, salary, hire_date) VALUES
('أحمد محمد', 'المبيعات', 5000, '2020-01-15'),
('فاطمة علي', 'التسويق', 6000, '2019-03-20'),
('يوسف خالد', 'التطوير', 7500, '2021-06-10'),
('ليلى عبدالله', 'المبيعات', 5500, '2022-01-05'),
('محمد حسن', 'التطوير', 8000, '2018-08-12'),
('سارة ناصر', 'التسويق', 4800, '2023-02-28');

INSERT INTO departments VALUES
(1, 'المبيعات', 1, 100000),
(2, 'التسويق', 2, 150000),
(3, 'التطوير', 5, 200000);

INSERT INTO projects VALUES
(1, 'موقع إلكتروني جديد', 'التطوير', 50000, '2024-01-01'),
(2, 'حملة تسويقية', 'التسويق', 30000, '2024-02-01'),
(3, 'توسعة المبيعات', 'المبيعات', 25000, '2024-03-01');
```

- بدون `Subqueries`:

```sql
SELECT name, salary
FROM employees
WHERE salary > AVG(salary);  -- ❌ خطأ!
-- دوال التجميع تعمل على مجموعات من البيانات وليس على صفوف فردية. جملة WHERE تعمل على كل صف على حدة قبل التجميع.
-- AVG(salary) تحتاج إلى حساب متوسط كل الرواتب، لكن WHERE تحاول تطبيق هذا على كل صف فردي.
```

- مع `Subqueries`:

```sql
SELECT name, salary
FROM employees
WHERE salary > (SELECT AVG(salary) FROM employees);
```

- استخدام `HAVING` (مع `GROUP BY`):

```sql
-- إذا كنت تريد متوسط لكل قسم
SELECT department, AVG(salary) as avg_salary
FROM employees
GROUP BY department
HAVING AVG(salary) > 5000;  -- ✅ HAVING يعمل مع دوال التجميع

-- عدد الموظفين في كل قسم
SELECT department, COUNT(*) as employee_count
FROM employees
GROUP BY department
HAVING COUNT(*) > 1;  -- ✅ HAVING يعمل مع COUNT
```

- استخدام `JOIN` مع `Subquery`:

```sql
-- للمقارنة مع متوسط القسم
SELECT e1.name, e1.department, e1.salary, e2.avg_dept_salary
FROM employees e1
JOIN (
    SELECT department, AVG(salary) as avg_dept_salary
    FROM employees
    GROUP BY department
) e2 ON e1.department = e2.department
WHERE e1.salary > e2.avg_dept_salary;
```

--

تحليل الاستعلام خطوة بخطوة

1. **Subquery الداخلية**

    ```sql
    SELECT department, AVG(salary) as avg_dept_salary
    FROM employees
    GROUP BY department
    ```

    **ما يفعله:**
    - يحسب متوسط الراتب (`AVG(salary)`) لكل قسم (`department`) في عمود `avg_dept_salary`

    - بدون `GROUP BY` يحسب متوسط جميع الأقسام

    - يرجع جدولاً مؤقتاً يحتوي على:
      - اسم القسم
      - متوسط راتب القسم

    - `department` في `SELECT`: يعرض اسم القسم ليتم ربطه مع `department` بجدول الموظفين

    - `department` في `GROUP BY`: يجمّع حسب القسم

2. **الـ JOIN الرئيسي**

    ```sql
    FROM employees e1
    JOIN (...) e2 ON e1.department = e2.department
    ```

    - `e1`: جدول الموظفين الأصلي
    - `e2`: الجدول المؤقت الناتج من `Subquery` (اسم القسم ومتوسط راتبه)
    - الربط يتم بناءً على اسم القسم (في جدول الموظفين الأصلي والجدول المؤقت)

3. **الشرط WHERE**

    ```sql
    WHERE e1.salary > e2.avg_dept_salary
    ```

    - يفلتر النتائج ليعرض فقط الموظفين الذين راتبهم أعلى من متوسط قسمهم

--

- قاعدة ذهبية:
  - `WHERE` → للشروط على صفوف فردية (لا تقبل دوال تجميع)
  - `HAVING` → للشروط على مجموعات (تقبل دوال تجميع بعد GROUP BY)
  - `Subquery` → عندما تحتاج قيمة مجمعة في شرط WHERE

- 🔍 **أنواع الـ Subqueries**

1. **Single-Row Subquery** (تُعيد صف واحد)

    ```sql
    -- الموظف الذي راتبه أعلى من متوسط الرواتب
    SELECT name, salary
    FROM employees
    WHERE salary > (SELECT AVG(salary) FROM employees);
    ```

2. **Multiple-Row Subquery** (تُعيد عدة صفوف)

    ```sql
    -- الموظفون في الأقسام التي لديها مشاريع
    SELECT name, department
    FROM employees
    WHERE department IN (SELECT DISTINCT department FROM projects);
    ```

3. **Correlated Subquery** (مرتبط بالاستعلام الخارجي)

    ```sql
    -- الموظفون الذين رواتبهم أعلى من متوسط قسمهم
    SELECT e1.name, e1.department, e1.salary
    FROM employees e1
    WHERE salary > (
        SELECT AVG(e2.salary)
        FROM employees e2
        WHERE e2.department = e1.department
    );
    ```

📊 **استخدام الـ Subqueries في أماكن مختلفة**

- مع `SELECT`:

```sql
-- عرض اسم الموظف ومتوسط راتب قسمه
SELECT 
    name,
    department,
    salary,
    (SELECT AVG(salary) FROM employees e2 WHERE e2.department = e1.department) as avg_dept_salary
FROM employees e1;
```

- مع `FROM` (`Inline View`):

```sql
-- متوسط الراتب حسب القسم
SELECT department, avg_salary
FROM (
    SELECT department, AVG(salary) as avg_salary
    FROM employees
    GROUP BY department
) as dept_stats
WHERE avg_salary > 5500;
```

- مع `INSERT`:

```sql
-- إنشاء جدول للموظفين المتميزين
CREATE TABLE top_employees (
    name VARCHAR(100),
    department VARCHAR(50),
    salary DECIMAL(10,2)
);

-- إدراج الموظفين الذين رواتبهم فوق المتوسط
INSERT INTO top_employees
SELECT name, department, salary
FROM employees
WHERE salary > (SELECT AVG(salary) FROM employees);
```

- مع `UPDATE`:

```sql
-- زيادة رواتب الموظفين في الأقسام التي لديها ميزانية عالية
UPDATE employees
SET salary = salary * 1.1
WHERE department IN (
    SELECT dept_name 
    FROM departments 
    WHERE budget > 120000
);
```

- مع `DELETE`:

```sql
-- حذف الموظفين في الأقسام التي لا تحتوي على مشاريع
DELETE FROM employees
WHERE department NOT IN (
    SELECT DISTINCT department 
    FROM projects
);
```

🎯 **أمثلة عملية متقدمة**

- المثال 1: أعلى راتب في كل قسم

```sql
SELECT name, department, salary
FROM employees e1
WHERE salary = (
    SELECT MAX(salary)
    FROM employees e2
    WHERE e2.department = e1.department
);
```

- المثال 2: الأقسام التي متوسط رواتبها فوق المتوسط العام

```sql
SELECT department, AVG(salary) as avg_salary
FROM employees
GROUP BY department
HAVING AVG(salary) > (SELECT AVG(salary) FROM employees);
```

- المثال 3: استخدام `EXISTS`:

```sql
-- الأقسام التي لديها موظفون
SELECT dept_name
FROM departments d
WHERE EXISTS (
    SELECT 1
    FROM employees e
    WHERE e.department = d.dept_name
);
```

كيف يعمل:
    `EXISTS`: تتحقق إذا كان الاستعلام الداخلي يعيد أي نتائج
    `SELECT 1`: تعني "أعط أي قيمة" (لا تهم القيمة، المهم وجود سجلات)
    الترجمة: "أعطني أسماء الأقسام التي لديها موظفون على الأقل"

مقارنة مع `IN`:

```sql
-- باستخدام IN
SELECT dept_name FROM departments
WHERE dept_name IN (SELECT department FROM employees);

-- باستخدام EXISTS (أكثر كفاءة غالباً)
SELECT dept_name FROM departments d
WHERE EXISTS (SELECT 1 FROM employees e WHERE e.department = d.dept_name);
```

- ⚡ **بدائل الـ Subqueries باستخدام JOIN**

- تحويل `Subquery` إلى `JOIN`:

```sql
-- باستخدام Subquery
SELECT name, department
FROM employees
WHERE department IN (SELECT dept_name FROM departments WHERE budget > 120000);

-- باستخدام JOIN (أكثر كفاءة غالباً)
SELECT DISTINCT e.name, e.department
FROM employees e
JOIN departments d ON e.department = d.dept_name
WHERE d.budget > 120000;
```

- 🚀 **أفضل الممارسات**

1. **استخدم JOIN عندما يكون ذلك ممكناً**

    ```sql
    -- ❌ غير مفضل
    SELECT name 
    FROM employees 
    WHERE department IN (SELECT dept_name FROM departments WHERE budget > 100000);

    -- ✅ أفضل
    SELECT e.name 
    FROM employees e
    JOIN departments d ON e.department = d.dept_name
    WHERE d.budget > 100000;
    ```

2. **استخدم INDEX على الأعمدة المستخدمة في WHERE**

    ```sql
    CREATE INDEX idx_department ON employees(department);
    CREATE INDEX idx_salary ON employees(salary);
    ```

3. **تجنب الـ Subqueries غير الضرورية في SELECT**

    ```sql
    -- ❌ غير فعال
    SELECT 
        name,
        (SELECT COUNT(*) FROM employees e2 WHERE e2.department = e1.department) as dept_count
    FROM employees e1;

    -- ✅ أفضل
    SELECT 
        e1.name,
        e2.dept_count
    FROM employees e1
    JOIN (
        SELECT department, COUNT(*) as dept_count
        FROM employees
        GROUP BY department
    ) e2 ON e1.department = e2.department;
    ```

📋 **تمارين عملية**

- التمرين 1: الموظفون الجدد الذين انضموا بعد آخر موظف في قسمهم

```sql
SELECT name, department, hire_date
FROM employees e1
WHERE hire_date > (
    SELECT MAX(hire_date)
    FROM employees e2
    WHERE e2.department = e1.department
    AND e2.id != e1.id
);
```

- التمرين 2: الأقسام التي لديها أكثر من موظفين

```sql
SELECT dept_name
FROM departments d
WHERE (
    SELECT COUNT(*) 
    FROM employees e 
    WHERE e.department = d.dept_name
) > 2;
```

- 💡 **نصائح مهمة**

1. **اختبر الـ Subquery منفردة أولاً**
2. **استخدم EXPLAIN لتحليل الأداء**
3. **تجنب الـ Subqueries المترابطة في جداول كبيرة**
4. **فكر في استخدام Temporary Tables للعمليات المعقدة**

--

#### Stored Procedures - الإجراءات المخزنة

الإجراءات المخزنة هي برامج أو دوال تُخزن في قاعدة البيانات وتُنفَّذ على الخادم. تشبه الدوال في لغات البرمجة العادية ولكنها تعمل داخل `MySQL`.

**ما هي الإجراءات المخزنة؟:**

- ✅ كود `SQL` يُخزن في قاعدة البيانات
- ✅ يُنفذ على خادم قاعدة البيانات
- ✅ يمكن استدعاؤه من التطبيقات المختلفة
- ✅ يقبل معاملات إدخال ويُعيد نتائج

**لماذا نستخدم Stored Procedures؟:**

*المزايا:*

- 🚀 **أداء أفضل**: التنفيذ على الخادم يقلل من حركة الشبكة
- 🛡️ **أمان**: إخفاء هيكل الجداول ومنح صلاحيات محدودة
- 🔄 **إعادة الاستخدام**: كود واحد لعدة تطبيقات
- 📊 **تناسق**: تنفيذ موحد للعمليات المشتركة

*العيوب:*

- ⚠️ **تعقيد**: صعوبة `debugging` والصيانة
- 🔒 **ربط بمزود**: صعوبة النقل بين أنظمة قواعد البيانات
- 💾 **استهلاك موارد**: على خادم قاعدة البيانات

**إنشاء الجداول والبيانات:**

*users:*

```sql
CREATE TABLE users (
    id INT PRIMARY KEY AUTO_INCREMENT,
    first_name VARCHAR(50) NOT NULL,
    last_name VARCHAR(50) NOT NULL,
    email VARCHAR(100) UNIQUE NOT NULL,
    salary DECIMAL(10,2) DEFAULT 0,
    status VARCHAR(20) DEFAULT 'active',
    points INT DEFAULT 0,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

INSERT INTO users (first_name, last_name, email, salary, points) VALUES
('أحمد', 'محمد', 'ahmed@example.com', 5000, 1200),
('فاطمة', 'علي', 'fatima@example.com', 6000, 800),
('يوسف', 'خالد', 'youssef@example.com', 4500, 300),
('سارة', 'عمر', 'sara@example.com', 5500, 1500);
```

*products:*

```sql
CREATE TABLE products (
    product_id INT PRIMARY KEY AUTO_INCREMENT,
    product_name VARCHAR(100) NOT NULL,
    category VARCHAR(50),
    price DECIMAL(10,2) NOT NULL,
    stock_quantity INT DEFAULT 0
);

INSERT INTO products (product_name, category, price, stock_quantity) VALUES
('لابتوب ديل', 'إلكترونيات', 3000, 10),
('ماوس لاسلكي', 'إلكترونيات', 150, 50),
('كتب برمجة', 'كتب', 80, 100),
('طابعة كانون', 'أجهزة مكتبية', 800, 15);
```

*orders:*

```sql
CREATE TABLE orders (
    order_id INT PRIMARY KEY AUTO_INCREMENT,
    customer_id INT,
    order_date DATE NOT NULL,
    total_amount DECIMAL(10,2),
    status VARCHAR(20) DEFAULT 'pending'
);

INSERT INTO orders (customer_id, order_date, total_amount, status) VALUES
(1, '2024-01-15', 3150, 'completed'),
(2, '2024-01-16', 80, 'completed'),
(1, '2024-01-17', 150, 'pending');
```

*order_details:*

```sql
CREATE TABLE order_details (
    order_detail_id INT PRIMARY KEY AUTO_INCREMENT,
    order_id INT,
    product_id INT,
    quantity INT NOT NULL,
    unit_price DECIMAL(10,2) NOT NULL,
    FOREIGN KEY (order_id) REFERENCES orders(order_id),
    FOREIGN KEY (product_id) REFERENCES products(product_id)
);

INSERT INTO order_details (order_id, product_id, quantity, unit_price) VALUES
(1, 1, 1, 3000),
(1, 2, 1, 150),
(2, 3, 1, 80),
(3, 2, 1, 150);
```

**بناء الإجراء المخزن الأساسي:**

*إنشاء أول إجراء مخزن:*

```sql
DELIMITER //

CREATE PROCEDURE GetAllUsers()
BEGIN
    SELECT * FROM users;
END //

DELIMITER ;
```

--

**أنواع المعاملات (Parameters):**

--

*1. معاملات الإدخال (IN) - الافتراضي:*

```sql
DELIMITER //

CREATE PROCEDURE GetUserByEmail(IN user_email VARCHAR(100))
BEGIN
    SELECT * FROM users WHERE email = user_email;
END //

DELIMITER ;

-- استدعاء إجراء بمعامل إدخال:
CALL GetUserByEmail('ahmed@example.com');
```

*2. معاملات الإخراج (OUT):*

```sql
DELIMITER //

CREATE PROCEDURE GetUserCount(OUT total_count INT)
BEGIN
    -- أضافة حقل total_count به عدد المستخدمين
    SELECT COUNT(*) INTO total_count FROM users;
END //

DELIMITER ;

-- استدعاء إجراء بمعامل إخراج:
-- تعريف متغير واستقبال الناتج
SET @count = 0;  -- هذه تهيئة للمتغير بقيمة ابتدائية
CALL GetUserCount(@count);
SELECT @count AS total_users;
```

*3. معاملات الإدخال والإخراج (INOUT):*

```sql
DELIMITER //

CREATE PROCEDURE IncreaseSalary(
    INOUT salary_amount DECIMAL(10,2), 
    IN increase_percent INT
)
BEGIN
    SET salary_amount = salary_amount * (1 + increase_percent / 100);
    -- هذا الإجراء يجري عملية حسابية فقط لحساب زيادة الراتب بنسبة مئوية
    -- لا يستعلم من أي جدول في قاعدة البيانات
    -- مثال: إذا كان الراتب 5000 ونسبة الزيادة (10%)
    -- increase_percent / 100 = 10 / 100 = 0.10
    -- 1 + 0.10 = 1.10
    -- salary_amount * 1.10 = 5000 * 1.10 = 5500
    -- إذاً: الراتب الجديد = الراتب القديم × (1 + نسبة الزيادة ÷ 100)
END //

DELIMITER ;

-- استدعاء إجراء بمعامل INOUT:
SET @current_salary = 5000;  -- راتب افتراضي
CALL IncreaseSalary(@current_salary, 10);  -- زيادة (10%)
SELECT @current_salary AS new_salary; -- 5500
```

**HANDLERS (معالجات الأخطاء):**

- `HANDLERS`: تتعامل مع الأخطاء التي قد تحدث أثناء تنفيذ الإجراء

- أنواع `HANDLERS` الرئيسية:
    1. `EXIT HANDLER`: يخرج من الإجراء بعد معالجة الخطأ
    2. `CONTINUE HANDLER`: يستمر في التنفيذ بعد معالجة الخطأ

- أمثلة على أنواع الأخطاء:

```sql
DECLARE EXIT HANDLER FOR SQLEXCEPTION          -- لأي خطأ في SQL
DECLARE EXIT HANDLER FOR SQLWARNING            -- للتحذيرات
DECLARE EXIT HANDLER FOR NOT FOUND             -- عندما لا توجد نتائج
DECLARE EXIT HANDLER FOR 1062                  -- لخطأ مكرر (DUPLICATE ENTRY)

-- مثال عملي:
DECLARE EXIT HANDLER FOR SQLEXCEPTION
BEGIN
    ROLLBACK;  -- تراجع عن العمليات
    -- يمكنك إضافة أي كود تريد تنفيذه عند حدوث الخطأ
    INSERT INTO error_log (error_message, error_time) 
    VALUES ('حدث خطأ في الإجراء', NOW());
END;
```

**أمثلة عملية متقدمة:**

*مثال 1: إجراء مع معاملات متعددة ومعالجة الأخطاء:*

```sql
DELIMITER //

CREATE PROCEDURE AddNewUser(
    IN p_first_name VARCHAR(50),
    IN p_last_name VARCHAR(50),
    IN p_email VARCHAR(100),
    OUT p_message VARCHAR(100)
)
BEGIN
    -- معالج الأخطاء: إذا حدث أي خطأ في SQL
    DECLARE EXIT HANDLER FOR SQLEXCEPTION
    BEGIN
        ROLLBACK;                    -- تراجع عن جميع العمليات إذا حدث خطأ
        SET p_message = 'Error: Failed to add user';  -- ضع رسالة الخطأ
    END;
    
    START TRANSACTION;  -- ابدأ مجموعة من العميات (إما تنجح جميعاً أو تفشل جميعاً)
    
    -- التحقق من عدم وجود البريد مسبقاً
    IF EXISTS (SELECT 1 FROM users WHERE email = p_email) THEN
    -- إذا كان البريد موجود مسبقاً
        SET p_message = 'Error: Email already exists';
    ELSE
        -- إذا كان البريد غير موجود، أضف المستخدم
        INSERT INTO users (first_name, last_name, email, created_at)
        VALUES (p_first_name, p_last_name, p_email, NOW());
        
        SET p_message = 'User added successfully';
        COMMIT;  -- يؤكد وينفذ جميع العمليات التي بدأت بـ START TRANSACTION فيحفظ التغييرات بشكل دائم في قاعدة البيانات
    END IF;
    
END //

DELIMITER ;

-- إضافة مستخدم جديد (ناجح)
-- تهيئة متغير الرسالة
SET @message = '';

-- استدعاء الإجراء بإضافة مستخدم جديد
CALL AddNewUser('محمد', 'السعيد', 'mohamed@example.com', @message);

-- عرض الرسالة
SELECT @message AS addition_result;

-- محاولة إضافة بريد مكرر (فاشل)
SET @message = '';
CALL AddNewUser('علي', 'حسن', 'ahmed@example.com', @message); -- البريد موجود مسبقاً
SELECT @message AS addition_result;

-- عرض جميع المستخدمين بعد الإضافات
SELECT * FROM users;
```

*مثال 2: إجراء مع عمليات معقدة:*

```sql
DELIMITER //

CREATE PROCEDURE ProcessOrder(
    IN p_customer_id INT,
    IN p_product_id INT,
    IN p_quantity INT
)
BEGIN
    -- إنشاء متغيرات مؤقتة لتخزين القيم
    DECLARE v_price DECIMAL(10,2);    -- لتخزين سعر المنتج
    DECLARE v_total DECIMAL(10,2);    -- لتخزين الإجمالي
    DECLARE v_order_id INT;           -- لتخزين رقم الطلب الجديد
    
    -- معالج الأخطاء: إذا حدث أي خطأ في SQL
    DECLARE EXIT HANDLER FOR SQLEXCEPTION
    BEGIN
        ROLLBACK;    -- تراجع عن جميع العمليات
        RESIGNAL;    -- أعد إظهار الخطأ للبرنامج المستدعي
    END;
    
    START TRANSACTION;  -- ابدأ مجموعة من العميات (إما تنجح جميعاً أو تفشل جميعاً)
    
    -- الحصول على سعر المنتج من خلال id
    SELECT price INTO v_price FROM products WHERE product_id = p_product_id;
    
    -- حساب الإجمالي
    SET v_total = v_price * p_quantity; -- متغير الإجمالي المؤقت = سعر المنتج صاحب id × الكمية المدخلة
    
    -- إنشاء طلب جديد
    INSERT INTO orders (customer_id, order_date, total_amount)
    VALUES (p_customer_id, NOW(), v_total); -- id العميل وتاريخ الطلب والسعر الاجمالي
    
    -- الحصول على رقم الطلب الجديد
    SET v_order_id = LAST_INSERT_ID();  -- LAST_INSERT_ID() ترجع آخر قيمة تم إنشاؤها تلقائياً (AUTO_INCREMENT)
    
    -- إضافة تفاصيل الطلب
    INSERT INTO order_details (order_id, product_id, quantity, unit_price)
    VALUES (v_order_id, p_product_id, p_quantity, v_price); -- رقم الطلب الجديد و id المنتج والكمية والسعر الإجمالي
    
    -- تحديث المخزون
    UPDATE products 
    -- إنقاص الكمية التي تم شراؤها من المخزون
    SET stock_quantity = stock_quantity - p_quantity
    WHERE product_id = p_product_id;
    
    COMMIT;  -- يؤكد وينفذ جميع العمليات
    
END //

DELIMITER ;

-- عرض المنتجات والمخزون:
SELECT product_id, product_name, price, stock_quantity 
FROM products;

-- عرض المستخدمين:
SELECT id, first_name, last_name FROM users;

-- طلب ناجح (كمية متوفرة)
-- معالجة طلب: المستخدم 1 يطلب 2 من المنتج 2 (الماوس)
CALL ProcessOrder(1, 2, 2);

-- عرض النتائج
SELECT '✅ The request was successfully completed.' AS result;

-- عرض الطلب الجديد
SELECT * FROM orders WHERE order_id = LAST_INSERT_ID();

-- عرض تفاصيل الطلب
SELECT * FROM order_details WHERE order_id = LAST_INSERT_ID();

-- عرض المخزون المحدث
SELECT product_id, product_name, stock_quantity 
FROM products WHERE product_id = 2;

-- محاولة طلب 100 من المنتج 1 (لابتوب) - قد يفشل إذا المخزون غير كافي
CALL ProcessOrder(3, 1, 100);
```

*التحقق النهائي من جميع البيانات:*

```sql
-- عرض جميع الطلبات:
SELECT o.order_id, 
       u.first_name, 
       u.last_name,
       o.order_date, 
       o.total_amount,
       o.status
FROM orders o
JOIN users u ON o.customer_id = u.id;

-- عرض جميع تفاصيل الطلبات:
SELECT od.order_detail_id,
       od.order_id,
       p.product_name,
       od.quantity,
       od.unit_price,
       (od.quantity * od.unit_price) as total
FROM order_details od
JOIN products p ON od.product_id = p.product_id;

-- عرض المخزون المتبقي:
SELECT product_id, product_name, price, stock_quantity
FROM products
ORDER BY product_id;
```

*اختبار سيناريو متكامل:*

```sql
-- 1. إضافة مستخدم جديد
SET @msg1 = '';
CALL AddNewUser('نور', 'الزيد', 'noor@example.com', @msg1);
SELECT @msg1 AS user_add_result;

-- 2. معالجة طلب لهذا المستخدم الجديد
-- أولاً نحصل على ID المستخدم الجديد
SET @new_user_id = LAST_INSERT_ID();
SELECT @new_user_id AS id_new_user;

-- 3. معالجة طلب للمستخدم الجديد
CALL ProcessOrder(@new_user_id, 4, 1); -- طلب طابعة

-- 4. عرض النتائج النهائية
SELECT '🎉 The scenario was completed successfully.' AS result;

SELECT u.first_name, 
       u.last_name, 
       p.product_name,
       od.quantity,
       o.total_amount
FROM orders o
JOIN users u ON o.customer_id = u.id
JOIN order_details od ON o.order_id = od.order_id
JOIN products p ON od.product_id = p.product_id
WHERE u.id = @new_user_id;
```

**التحكم في التدفق (Control Flow):**

- عرض المستخدمين الحاليين قبل التشغيل:

```sql
SELECT id, first_name, last_name, email, status, points 
FROM users 
ORDER BY id;
```

*استخدام IF:*

```sql
DELIMITER //

CREATE PROCEDURE CheckUserStatus(IN user_id INT)
BEGIN
    DECLARE user_status VARCHAR(20);
    
    SELECT status INTO user_status FROM users WHERE id = user_id;
    
    IF user_status = 'active' THEN
        SELECT 'User is active' AS message;
    ELSEIF user_status = 'inactive' THEN
        SELECT 'User is inactive' AS message;
    ELSE
        SELECT 'Unknown status' AS message;
    END IF;
    
END //

DELIMITER ;

--  التحقق من حالة مستخدم نشط
CALL CheckUserStatus(1);  -- User is active

-- التحقق من حالة مستخدم غير نشط
-- أولاً نغير حالة مستخدم إلى inactive
UPDATE users SET status = 'inactive' WHERE id = 2;

-- ثم نتحقق
CALL CheckUserStatus(2);  -- User is inactive

-- التحقق من حالة غير معروفة
-- نغير حالة مستخدم إلى قيمة غير متوقعة
UPDATE users SET status = 'pending' WHERE id = 3;

-- ثم نتحقق
CALL CheckUserStatus(3);  -- Unknown status
```

*استخدام CASE:*

```sql
DELIMITER //

CREATE PROCEDURE GetUserLevel(IN user_id INT)
BEGIN
    DECLARE user_points INT;
    
    SELECT points INTO user_points FROM users WHERE id = user_id;
    
    CASE 
        WHEN user_points >= 1000 THEN
            SELECT 'Gold' AS level;
        WHEN user_points >= 500 THEN
            SELECT 'Silver' AS level;
        WHEN user_points >= 100 THEN
            SELECT 'Bronze' AS level;
        ELSE
            SELECT 'Regular' AS level;
    END CASE;
    
END //

DELIMITER ;

--  التحقق من نقاط المستخدمين الحاليين:
SELECT id, first_name, points FROM users ORDER BY points DESC;

-- مستخدم مستوى Gold (1000+ نقطة)
UPDATE users SET points = 1200 WHERE id = 1;
CALL GetUserLevel(1);  -- Gold

-- مستخدم مستوى Silver (500-999 نقطة)
UPDATE users SET points = 800 WHERE id = 2;
CALL GetUserLevel(2);  -- Silver

-- مستخدم مستوى Bronze (100-499 نقطة)
UPDATE users SET points = 300 WHERE id = 3;
CALL GetUserLevel(3);  -- Bronze

-- مستخدم مستوى Regular (أقل من 100 نقطة)
UPDATE users SET points = 50 WHERE id = 4;
CALL GetUserLevel(4);
```

*استخدام الحلقات (LOOPS):*

```sql
DELIMITER //

CREATE PROCEDURE GenerateTestUsers()
BEGIN
-- هذه الحلقة تنشئ 10 مستخدمين تجريبين تلقائياً
DECLARE i INT DEFAULT 1;  -- متغير عداد يبدأ من 1

WHILE i <= 10 DO  -- كرر طالما (i) أقل من أو يساوي (10)
    
    -- أدخل مستخدم جديد مع دمج القيم
    INSERT INTO users (first_name, last_name, email, created_at)
    VALUES (
        CONCAT('User', i),      -- أول اسم: User1, User2, ... User10
        CONCAT('Test', i),      -- آخر اسم: Test1, Test2, ... Test10  
        CONCAT('user', i, '@test.com'),  -- بريد: user1@test.com, ...
        NOW()                   -- وقت الإنشاء الحالي
    );
    
    SET i = i + 1;  -- زد العداد بمقدار 1
END WHILE;
    
END //

DELIMITER ;

-- التحقق من عدد المستخدمين قبل التشغيل:
SELECT COUNT(*) AS current_number_of_users FROM users;

-- تشغيل الإجراء لإنشاء 10 مستخدمين تجريبيين
CALL GenerateTestUsers();

-- عرض رسالة نجاح
SELECT '✅ 10 trial users successfully created' AS result;
```

*التحقق من النتائج:*

```sql
-- عرض المستخدمين الجدد:
SELECT id, first_name, last_name, email, created_at 
FROM users 
ORDER BY id DESC 
LIMIT 10;  -- عرض آخر 10 مستخدمين تم إضافتهم

-- التحقق من العدد الكلي:
SELECT COUNT(*) AS total_number_of_users FROM users;
```

*اختبار شامل لجميع الإجراءات:*

```sql
-- 1. تعيين نقاط عشوائية للمستخدمين الجدد
UPDATE users SET points = FLOOR(RAND() * 1500) WHERE id > 5;

-- 2. تعيين حالات عشوائية
UPDATE users SET status = 
    CASE 
        WHEN RAND() > 0.5 THEN 'active' 
        ELSE 'inactive' 
    END 
WHERE id > 5;

-- 3. اختبار CheckUserStatus للمستخدمين الجدد
SELECT '=== اختبار حالة المستخدمين ===' AS title;
CALL CheckUserStatus(6);
CALL CheckUserStatus(8);
CALL CheckUserStatus(12);

-- 4. اختبار GetUserLevel للمستخدمين الجدد
SELECT '=== اختبار مستويات المستخدمين ===' AS title;
CALL GetUserLevel(7);
CALL GetUserLevel(9);
CALL GetUserLevel(11);

-- 5. عرض تقرير نهائي
SELECT '=== التقرير النهائي ===' AS title;
SELECT 
    id,
    first_name,
    last_name,
    email,
    status,
    points,
    CASE 
        WHEN points >= 1000 THEN 'Gold'
        WHEN points >= 500 THEN 'Silver' 
        WHEN points >= 100 THEN 'Bronze'
        ELSE 'Regular'
    END AS calculated_level
FROM users 
WHERE id > 5
ORDER BY id;
```

**إدارة الإجراءات المخزنة:**

*عرض الإجراءات المخزنة:*

```sql
-- عرض جميع الإجراءات
SHOW PROCEDURE STATUS;

-- عرض إجراء محدد
SHOW CREATE PROCEDURE GetUserByEmail;
```

*تعديل الإجراء المخزن:*

```sql
-- حذف المستخدمين التجريبيين فقط
DELETE FROM users WHERE email LIKE 'user%@test.com';

-- التحقق من الحذف
SELECT COUNT(*) AS number_of_users_after_deletion FROM users;

-- لا يوجد MODIFY PROCEDURE، يجب حذف وإعادة إنشاء
DROP PROCEDURE IF EXISTS GetUserByEmail;

DELIMITER //
CREATE PROCEDURE GetUserByEmail(IN user_email VARCHAR(100))
BEGIN
    SELECT id, first_name, last_name, email 
    FROM users 
    WHERE email = user_email;
END //
```

*حذف الإجراء المخزن:*

```sql
DROP PROCEDURE GetUserByEmail;
```

**أفضل الممارسات:**

*✅ نصائح للاستخدام الفعال:*

1. استخدم أسماء واضحة ومعبرة
2. أضف تعليقات توضيحية
3. تعامل مع الأخطاء باستخدام `HANDLERS`
4. استخدم المعاملات للعمليات المتعددة
5. قلل من كمية البيانات المعادة

*❌ ما يجب تجنبه:*

1. لا تكتب إجراءات معقدة جداً
2. تجنب العمليات التي تستغرق وقتاً طويلاً
3. لا تنسى إغلاق المؤقتات (Cursors)
4. لا تستخدم للإجراءات البسيطة

**مثال متكامل من الحياة الواقعية:**

```sql
DELIMITER //

CREATE PROCEDURE MonthlySalesReport(
    IN report_month INT,
    IN report_year INT,
    OUT total_sales DECIMAL(12,2),
    OUT total_orders INT,
    OUT top_product VARCHAR(100)
)
BEGIN
    DECLARE EXIT HANDLER FOR SQLEXCEPTION
    BEGIN
        ROLLBACK;
        RESIGNAL;
    END;
    
    START TRANSACTION;
    
    -- حساب إجمالي المبيعات
    SELECT COALESCE(SUM(total_amount), 0) INTO total_sales
    FROM orders 
    WHERE MONTH(order_date) = report_month 
    AND YEAR(order_date) = report_year;
    
    -- حساب عدد الطلبات
    SELECT COUNT(*) INTO total_orders
    FROM orders 
    WHERE MONTH(order_date) = report_month 
    AND YEAR(order_date) = report_year;
    
    -- تحديد المنتج الأكثر مبيعاً
    SELECT p.product_name INTO top_product
    FROM order_details od
    JOIN products p ON od.product_id = p.product_id
    JOIN orders o ON od.order_id = o.order_id
    WHERE MONTH(o.order_date) = report_month 
    AND YEAR(o.order_date) = report_year
    GROUP BY p.product_id, p.product_name
    ORDER BY SUM(od.quantity) DESC
    LIMIT 1;
    
    COMMIT;
    
END //

DELIMITER ;
```

**الاستخدام:**

```sql
-- استدعاء التقرير الشهري
SET @sales = 0;
SET @orders = 0;
SET @product = '';

CALL MonthlySalesReport(12, 2024, @sales, @orders, @product);

SELECT @sales AS total_sales, @orders AS total_orders, @product AS top_product;
```

--

#### Normalization - التطبيع

التطبيع هو عملية تنظيم البيانات في قاعدة البيانات بشكل منهجي لتقليل التكرار وتحسين تكامل البيانات. الهدف الرئيسي هو إنشاء جداول وعلاقات بينها بطريقة تحمي البيانات وتجعل القاعدة أكثر مرونة.

**أهداف التطبيع:**

- ✅ تقليل تكرار البيانات
- ✅ منع التناقض في البيانات
- ✅ تسهيل صيانة القاعدة
- ✅ تحسين كفاءة الاستعلامات

**أشكال التطبيع الرئيسية:**

**1. الصيغة الأولى (1NF)**
**المتطلبات:**

- كل عمود يحتوي على قيم ذرية (غير قابلة للتقسيم)
- كل سجل فريد (لا توجد صفوف مكررة)

**مثال:**

```sql
-- ❌ غير مطبع
| OrderID | Products       |
|---------|----------------|
| 1       | Laptop, Mouse  |

-- ✅ مطبع (1NF)
| OrderID | Product  |
|---------|----------|
| 1       | Laptop   |
| 1       | Mouse    |
```

**2. الصيغة الثانية (2NF)**
**المتطلبات:**

- تحقيق `1NF`
- جميع الأعمدة غير المفتاحية تعتمد على المفتاح الرئيسي كاملاً

**مثال:**

```sql
-- ❌ غير مطبع (سعر المنتج يعتمد على ProductID فقط)
| OrderID | ProductID | ProductName | Price |
|---------|-----------|-------------|-------|

-- ✅ مطبع (2NF)
-- جدول الطلبات
| OrderID | ProductID | Quantity |
|---------|-----------|----------|

-- جدول المنتجات
| ProductID | ProductName | Price |
|-----------|-------------|-------|
```

**3. الصيغة الثالثة (3NF)**
**المتطلبات:**

- تحقيق `2NF`
- لا توجد تبعيات متعدية (جميع الأعمدة تعتمد فقط على المفتاح الرئيسي)

**مثال:**

```sql
-- ❌ غير مطبع (المدينة تعتمد على الرمز البريدي)
| CustomerID | Name  | ZipCode | City     |
|------------|-------|---------|----------|

-- ✅ مطبع (3NF)
-- جدول العملاء
| CustomerID | Name  | ZipCode |
|------------|-------|---------|

-- جدول المناطق
| ZipCode | City     |
|---------|----------|
```

**مثال عملي متكامل:**

*قبل التطبيع:*

```sql
CREATE TABLE sales (
    order_id INT,
    customer_name VARCHAR(100),
    customer_phone VARCHAR(20),
    product_name VARCHAR(100),
    product_category VARCHAR(50),
    price DECIMAL(10,2),
    quantity INT
);
```

*بعد التطبيع:*

```sql
-- جدول العملاء
CREATE TABLE customers (
    customer_id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100),
    phone VARCHAR(20)
);

-- جدول المنتجات
CREATE TABLE products (
    product_id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100),
    category VARCHAR(50),
    price DECIMAL(10,2)
);

-- جدول الطلبات
CREATE TABLE orders (
    order_id INT PRIMARY KEY AUTO_INCREMENT,
    customer_id INT,
    order_date DATE,
    FOREIGN KEY (customer_id) REFERENCES customers(customer_id)
);

-- جدول تفاصيل الطلبات
CREATE TABLE order_details (
    order_detail_id INT PRIMARY KEY AUTO_INCREMENT,
    order_id INT,
    product_id INT,
    quantity INT,
    FOREIGN KEY (order_id) REFERENCES orders(order_id),
    FOREIGN KEY (product_id) REFERENCES products(product_id)
);
```

**مزايا وعيوب التطبيع:**

*المزايا:*

- 🎯 تقليل تكرار البيانات
- 🛡️ تحسين تكامل البيانات
- 📊 استعلامات أكثر كفاءة
- 🔄 سهولة الصيانة والتحديث

*العيوب:*

- ⚠️ استعلامات أكثر تعقيداً (`JOIN` متعددة)
- ⏱️ أداء أبطأ في بعض عمليات القراءة
- 🏗️ تصميم أكثر تعقيداً

--

#### Important MySQL Queries For Backend Developer

**🔴 استعلامات MySQL الأساسية لكل Backend Developer:**

--

##### **استعلامات CRUD الأساسية**

- **الإنشاء (CREATE)**

```sql
-- إنشاء قاعدة بيانات
CREATE DATABASE company;

-- إنشاء جدول
CREATE TABLE users (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100) NOT NULL,
    email VARCHAR(100) UNIQUE,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-- إدراج بيانات
INSERT INTO users (name, email) VALUES ('أحمد', 'ahmed@example.com');
INSERT INTO users (name, email) VALUES 
('محمد', 'mohamed@example.com'),
('فاطمة', 'fatima@example.com');
```

- **القراءة (READ)**

```sql
-- اختيار جميع الأعمدة
SELECT * FROM users;

-- اختيار أعمدة محددة
SELECT id, name, email FROM users;

-- مع شرط WHERE
SELECT * FROM users WHERE id = 1;
SELECT * FROM users WHERE name LIKE 'أح%';
SELECT * FROM users WHERE created_at > '2024-01-01';

-- التحديد المميز
SELECT DISTINCT name FROM users;
```

- **التحديث (UPDATE)**

```sql
-- تحديث سجل واحد
UPDATE users SET name = 'أحمد محمد' WHERE id = 1;

-- تحديث multiple records
UPDATE users SET status = 'active' WHERE created_at < '2024-01-01';
```

- **الحذف (DELETE)**

```sql
-- حذف سجل محدد
DELETE FROM users WHERE id = 1;

-- حذف جميع السجلات
DELETE FROM users;

-- حذف جميع السجلات بشكل أسرع
TRUNCATE TABLE users;
```

--

##### **استعلامات التجميع والترتيب**

- **التجميع (Aggregation)**

```sql
-- COUNT, SUM, AVG, MAX, MIN
SELECT COUNT(*) AS total_users FROM users;
SELECT AVG(salary) AS avg_salary FROM employees;
SELECT MAX(salary) AS max_salary, MIN(salary) AS min_salary FROM employees;
SELECT SUM(amount) AS total_sales FROM orders;

-- مع GROUP BY
SELECT department, AVG(salary) AS avg_salary 
FROM employees 
GROUP BY department;

-- مع HAVING
SELECT department, AVG(salary) AS avg_salary 
FROM employees 
GROUP BY department 
HAVING AVG(salary) > 5000;
```

- **الترتيب والتصفية**

```sql
-- ORDER BY
SELECT * FROM users ORDER BY name ASC;
SELECT * FROM users ORDER BY created_at DESC;
SELECT * FROM users ORDER BY salary DESC, name ASC;

-- LIMIT و OFFSET
SELECT * FROM users LIMIT 10;
SELECT * FROM users LIMIT 10 OFFSET 20; -- لل pagination
SELECT * FROM users ORDER BY id DESC LIMIT 5; -- آخر 5 سجلات
```

--

##### **JOINS - الربط بين الجداول**

- **INNER JOIN**

```sql
SELECT u.name, o.order_date, o.amount
FROM users u
INNER JOIN orders o ON u.id = o.user_id;
```

- **LEFT JOIN**

```sql
SELECT u.name, o.order_date
FROM users u
LEFT JOIN orders o ON u.id = o.user_id;
```

- **RIGHT JOIN**

```sql
SELECT u.name, o.order_date
FROM users u
RIGHT JOIN orders o ON u.id = o.user_id;
```

- **Multiple Joins**

```sql
SELECT u.name, p.product_name, o.quantity
FROM users u
INNER JOIN orders o ON u.id = o.user_id
INNER JOIN products p ON o.product_id = p.id;
```

- **SELF JOIN**

```sql
SELECT e1.name AS employee, e2.name AS manager
FROM employees e1
LEFT JOIN employees e2 ON e1.manager_id = e2.id;
```

--

##### **الاستعلامات المتقدمة**

- **Subqueries**

```sql
-- في WHERE
SELECT name FROM users 
WHERE id IN (SELECT user_id FROM orders WHERE amount > 1000);

-- في SELECT
SELECT name, 
       (SELECT COUNT(*) FROM orders WHERE user_id = users.id) AS order_count
FROM users;

-- مع EXISTS
SELECT name FROM users u
WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
```

- **Common Table Expressions (CTE)**

```sql
WITH top_customers AS (
    SELECT user_id, SUM(amount) AS total_spent
    FROM orders 
    GROUP BY user_id 
    HAVING total_spent > 5000
)
SELECT u.name, tc.total_spent
FROM users u
INNER JOIN top_customers tc ON u.id = tc.user_id;

-- كيف يعمل:
-- top_customers هو استعلام مؤقت يجد العملاء الذين أنفقوا أكثر من 5000
-- ثم نستخدم هذا الاستعلام المؤقت كأنه جدول عادي
-- نربط النتائج بجدول المستخدمين للحصول على الأسماء
```

البديل بدون `CTE`:

```sql
-- نفس النتيجة ولكن أقل وضوحاً
SELECT u.name, SUM(o.amount) AS total_spent
FROM users u
INNER JOIN orders o ON u.id = o.user_id
GROUP BY u.id, u.name
HAVING SUM(o.amount) > 5000;
```

مزايا `CTE`:
    أكثر قابلية للقراءة
    يمكن إعادة استخدامه في نفس الاستعلام
    يدعم التكرار (`Recursive CTE`)

مثال متقدم:

```sql
WITH 
department_stats AS (
    SELECT department, AVG(salary) AS avg_salary
    FROM employees 
    GROUP BY department
),
top_departments AS (
    SELECT department 
    FROM department_stats 
    WHERE avg_salary > 7000
)
SELECT e.name, e.salary, e.department
FROM employees e
INNER JOIN top_departments td ON e.department = td.department;
```

--

##### **التعامل مع التواريخ والأوقات**

```sql
-- التاريخ الحالي
SELECT NOW(), CURDATE(), CURTIME();

-- استعلامات تاريخية
SELECT * FROM orders WHERE order_date = CURDATE();
SELECT * FROM orders WHERE order_date BETWEEN '2024-01-01' AND '2024-01-31';
SELECT * FROM orders WHERE YEAR(order_date) = 2024;
SELECT * FROM orders WHERE MONTH(order_date) = 1;

-- دوال التاريخ
SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);
SELECT DATE_SUB(NOW(), INTERVAL 1 MONTH);
SELECT DATEDIFF('2024-01-31', '2024-01-01');
SELECT DATE_FORMAT(NOW(), '%Y-%m-%d %H:%i:%s');
```

--

##### **التعامل مع النصوص**

```sql
-- دوال النصوص
SELECT CONCAT(first_name, ' ', last_name) AS full_name FROM users;
SELECT UPPER(name), LOWER(email) FROM users;
SELECT LENGTH(name) AS name_length FROM users;
SELECT SUBSTRING(email, 1, 5) FROM users;
SELECT REPLACE(description, 'old', 'new') FROM products;

-- البحث في النصوص
SELECT * FROM users WHERE name LIKE 'مح%';
SELECT * FROM users WHERE name LIKE '%أحمد%';
SELECT * FROM users WHERE name LIKE '_حمد'; -- حرف واحد ثم حمد
```

--

##### **التحكم في المعاملات (Transactions)**

```sql
-- معاملة بسيطة
START TRANSACTION;
UPDATE accounts SET balance = balance - 100 WHERE id = 1;
UPDATE accounts SET balance = balance + 100 WHERE id = 2;
COMMIT;

-- معاملة مع معالجة الأخطاء
START TRANSACTION;
BEGIN
    DECLARE EXIT HANDLER FOR SQLEXCEPTION
    BEGIN
        ROLLBACK;
        RESIGNAL;
    END;
    
    INSERT INTO orders (user_id, amount) VALUES (1, 100);
    UPDATE products SET stock = stock - 1 WHERE id = 5;
    COMMIT;
END;
```

--

##### **الإجراءات المخزنة والدوال**

- **Stored Procedures**

```sql
DELIMITER //
CREATE PROCEDURE GetUserOrders(IN user_id INT)
BEGIN
    SELECT * FROM orders WHERE user_id = user_id;
END //
DELIMITER ;

-- الاستدعاء
CALL GetUserOrders(1);
```

- **الدوال (Functions)**

```sql
DELIMITER //
CREATE FUNCTION GetTotalUserOrders(user_id INT) RETURNS INT
BEGIN
    DECLARE total INT;
    SELECT COUNT(*) INTO total FROM orders WHERE user_id = user_id;
    RETURN total;
END //
DELIMITER ;

-- الاستخدام
SELECT name, GetTotalUserOrders(id) AS total_orders FROM users;
```

- ***الدوال (Functions) vs Stored Procedures***

**الفرق الأساسي:**

| Aspect | الدوال (Functions) | الإجراءات المخزنة (Stored Procedures) |
|--------|-------------------|--------------------------------------|
| **الغرض** | حساب وإعادة قيمة | تنفيذ عمليات معقدة |
| **القيمة المعادة** | دائماً تعيد قيمة واحدة | يمكن أن تعيد 0، 1، أو multiple resultsets |
| **الاستخدام** | في SELECT statements | تُستدعى بـ CALL |
| **المعاملات** | Input parameters فقط | Input, Output, Inout parameters |
| **التعامل مع البيانات** | قراءة فقط (عادة) | قراءة وكتابة |

**مقارنة عملية:**

*الدالة (Function):*

```sql
DELIMITER //
CREATE FUNCTION GetUserOrderCount(user_id INT) RETURNS INT
BEGIN
    DECLARE order_count INT;
    SELECT COUNT(*) INTO order_count FROM orders WHERE user_id = user_id;
    RETURN order_count;
END //
DELIMITER ;

-- الاستخدام في SELECT
SELECT name, GetUserOrderCount(id) AS order_count FROM users;
```

*الإجراء المخزن (Stored Procedure):*

```sql
DELIMITER //
CREATE PROCEDURE GetUserOrders(IN user_id INT)
BEGIN
    SELECT * FROM orders WHERE user_id = user_id;
    SELECT COUNT(*) AS total_orders FROM orders WHERE user_id = user_id;
END //
DELIMITER ;

-- الاستخدام
CALL GetUserOrders(1);
```

--

##### **التحسين والأداء**

- **EXPLAIN لتحليل الاستعلامات**

```sql
EXPLAIN SELECT * FROM users WHERE email = 'test@example.com';
EXPLAIN ANALYZE SELECT * FROM users WHERE name LIKE 'أ%';
```

- **الفهارس (Indexes)**

```sql
-- إنشاء فهارس
CREATE INDEX idx_email ON users(email);
CREATE INDEX idx_name_age ON users(name, age);
CREATE UNIQUE INDEX idx_unique_email ON users(email);

-- عرض الفهارس
SHOW INDEX FROM users;

-- حذف الفهرس
DROP INDEX idx_email ON users;
```

- **EXPLAIN vs Indexes**

- *الفرق:*

| Aspect | EXPLAIN | Indexes |
|--------|---------|---------|
| **الغرض** | تحليل كيفية تنفيذ الاستعلام | تحسين سرعة الاستعلامات |
| **الفعل** | أداة تشخيص (Diagnostic) | أداة تحسين (Optimization) |
| **المخرجات** | خطة التنفيذ (Execution Plan) | بنية بيانات لتحسين الأداء |

- *التكامل بينهما:*

```sql
-- ١. تحليل استعلام بدون فهرس
EXPLAIN SELECT * FROM users WHERE email = 'test@example.com';
-- النتيجة: type = ALL (مسح كامل للجدول)

-- ٢. إنشاء فهرس
CREATE INDEX idx_email ON users(email);

-- ٣. تحليل نفس الاستعلام مع الفهرس
EXPLAIN SELECT * FROM users WHERE email = 'test@example.com';
-- النتيجة: type = ref (استخدام الفهرس)

-- ٤. تحليل متقدم
EXPLAIN ANALYZE SELECT * FROM users WHERE name LIKE 'أ%';
-- يعطي تحليل أداء مفصل مع أوقات التنفيذ
```

- *قراءة نتائج EXPLAIN:*
  - `type`: ALL = سيء, ref = جيد, const = ممتاز
  - `rows`: عدد الصفوف التي سيمسحها
  - `Extra`: معلومات إضافية (Using where, Using index, etc.)

--

##### **الاستعلامات الأمنية**

- **Prepared Statements**

```sql
-- في التطبيق (مثال في PHP)
$stmt = $pdo->prepare("SELECT * FROM users WHERE email = ? AND status = ?");
$stmt->execute([$email, $status]);
$user = $stmt->fetch();
```

- **الصلاحيات**

```sql
-- إنشاء مستخدم
CREATE USER 'app_user'@'localhost' IDENTIFIED BY 'password';

-- منح صلاحيات
GRANT SELECT, INSERT, UPDATE ON company.* TO 'app_user'@'localhost';

-- سحب صلاحيات
REVOKE DELETE ON company.* FROM 'app_user'@'localhost';
```

- *لماذا نستخدم الصلاحيات؟*
  - 🛡️ الأمان: منع الوصول غير المصرح به
  - 🎯 التحكم: تحديد ما يمكن لكل مستخدم فعله
  - 📊 الفصل: فصل مسؤوليات التطبيقات

- *سيناريوهات عملية:*

```sql
-- ١. مستخدم للتطبيق (قراءة وكتابة فقط)
CREATE USER 'app_user'@'localhost' IDENTIFIED BY 'password123';
GRANT SELECT, INSERT, UPDATE ON ecommerce.* TO 'app_user'@'localhost';
REVOKE DELETE ON ecommerce.* FROM 'app_user'@'localhost';

-- ٢. مستخدم للتقارير (قراءة فقط)
CREATE USER 'report_user'@'localhost' IDENTIFIED BY 'report123';
GRANT SELECT ON ecommerce.* TO 'report_user'@'localhost';

-- ٣. مستخدم للإدارة (جميع الصلاحيات)
CREATE USER 'admin_user'@'localhost' IDENTIFIED BY 'admin123';
GRANT ALL PRIVILEGES ON ecommerce.* TO 'admin_user'@'localhost';

-- ٤. عرض الصلاحيات
SHOW GRANTS FOR 'app_user'@'localhost';
```

- *الصلاحيات الشائعة:*
  - `SELECT` - قراءة البيانات
  - `INSERT` - إضافة بيانات جديدة
  - `UPDATE` - تعديل بيانات موجودة
  - `DELETE` - حذف بيانات
  - `CREATE` - إنشاء جداول وقواعد بيانات
  - `DROP` - حذف جداول وقواعد بيانات
  - `ALTER` - تعديل هيكل الجداول

--

##### **استعلامات الصيانة**

```sql
-- نسخ جدول (للاحتياط أو الاختبار)
CREATE TABLE users_backup AS SELECT * FROM users;
-- الاستخدام: نسخ بيانات قبل تحديث خطير


-- تحديث إحصاءات الجداول
ANALYZE TABLE users;
-- الغرض: مساعد مُحسِّن في اختيار أفضل خطط التنفيذ


-- إصلاح الجداول
REPAIR TABLE users;
-- الغرض: إصلاح تلف في الجداول (نادر الحدوث في InnoDB)


-- تحسين الجداول
OPTIMIZE TABLE users;
-- الغرض: إعادة تنظيم التخزين وتحسين الأداء بعد حذف/تحديث كميات كبيرة


-- عرض معلومات الجدول
SHOW TABLE STATUS LIKE 'users';
-- يعطي: حجم الجدول، عدد الصفوف، المحرك، etc.


DESCRIBE users;
-- يعطي: هيكل الجدول (الأعمدة، الأنواع، المفاتيح)
```

- *متى نستخدمها؟*
  - أسبوعياً: ANALYZE TABLE للجداول النشطة
  - شهرياً: OPTIMIZE TABLE للجداول كثيرة التحديث
  - قبل التحديثات الكبيرة: نسخ الجداول المهمة

--

##### **استعلامات متقدمة للبيانات الكبيرة**

--

- **Window Functions - دوال النوافذ**

- *الغرض: إجراء حسابات على مجموعات من الصفوف بدون تجميعها في صف واحد*

- *المشكلة التي تحلها:*
  - *بدون Window Functions:* عندما تريد ترتيب موظفين داخل كل قسم، تحتاج إلى استعلامات منفصلة أو كود معقد.
  - *مع Window Functions:* يمكنك فعل ذلك في استعلام واحد!

- *الفرق بين GROUP BY و Window Functions:*

| GROUP BY | Window Functions |
|----------|------------------|
| **يقلل الصفوف** - يعطي صفاً واحداً لكل مجموعة | **يحافظ على جميع الصفوف** - يضيف أعمدة جديدة |
| `COUNT(), SUM(), AVG()` | `RANK(), SUM() OVER(), AVG() OVER()` |
| **تجميع** | **حسابات على نوافذ** |

- *أمثلة عملية مفصلة:*

*البيانات الأساسية:*

```sql
-- جدول الموظفين
CREATE TABLE employees (
    id INT PRIMARY KEY,
    name VARCHAR(50),
    department VARCHAR(50),
    salary DECIMAL(10,2)
);

INSERT INTO employees VALUES
(1, 'أحمد', 'IT', 8000),
(2, 'محمد', 'IT', 7000),
(3, 'سارة', 'HR', 9000),
(4, 'فاطمة', 'HR', 8500),
(5, 'يوسف', 'IT', 7500),
(6, 'ليلى', 'Marketing', 6000);
```

- المثال 1: `RANK()` - الترتيب داخل الأقسام

```sql
SELECT 
    name,
    department,
    salary,
    RANK() OVER (PARTITION BY department ORDER BY salary DESC) as rank_in_department
FROM employees;

-- ترتيب الموظفين داخل كل قسم ضمن المجموعات
SELECT name, salary, 
       RANK() OVER (PARTITION BY department ORDER BY salary DESC) as the_rank
FROM employees;
```

النتيجة:

| name    | department | salary | rank_in_department |
|---------|------------|--------|-------------------|
| أحمد    | IT         | 8000   | 1                 |
| يوسف    | IT         | 7500   | 2                 |
| محمد    | IT         | 7000   | 3                 |
| سارة    | HR         | 9000   | 1                 |
| فاطمة   | HR         | 8500   | 2                 |
| ليلى    | Marketing  | 6000   | 1                 |

الشرح:

- `PARTITION BY department`: قسم البيانات إلى مجموعات حسب القسم
- `ORDER BY salary DESC`: رتب كل مجموعة حسب الراتب (تنازلي)
- `RANK()`: أعط رتبة لكل موظف داخل مجموعته

- المثال 2: `SUM() OVER()` - المجموع التراكمي

```sql
-- جدول المبيعات
CREATE TABLE sales (
    sale_date DATE,
    amount DECIMAL(10,2)
);

INSERT INTO sales VALUES
('2024-01-01', 1000),
('2024-01-02', 1500),
('2024-01-03', 800),
('2024-01-04', 2000);

SELECT 
    sale_date,
    amount,
    SUM(amount) OVER (ORDER BY sale_date) as running_total,
    AVG(amount) OVER (ORDER BY sale_date) as running_avg
FROM sales;

-- Running Total: المجموع التراكمي
SELECT order_date, amount,
    SUM(amount) OVER (ORDER BY order_date) as running_total
FROM orders;
```

النتيجة:

| sale_date   | amount | running_total | running_avg |
|-------------|--------|---------------|-------------|
| 2024-01-01  | 1000   | 1000          | 1000.00     |
| 2024-01-02  | 1500   | 2500          | 1250.00     |
| 2024-01-03  | 800    | 3300          | 1100.00     |
| 2024-01-04  | 2000   | 5300          | 1325.00     |

- المثال 3: دوال متقدمة

```sql
SELECT 
    name,
    department,
    salary,
    -- الراتب الأعلى في القسم
    MAX(salary) OVER (PARTITION BY department) as dept_max_salary,
    -- الراتب الأدنى في القسم  
    MIN(salary) OVER (PARTITION BY department) as dept_min_salary,
    -- الفرق بين راتب الموظف ومتوسط القسم
    salary - AVG(salary) OVER (PARTITION BY department) as diff_from_avg
FROM employees;
```

- *أنواع Window Functions الشائعة:*

- الترتيب: `RANK()`, `DENSE_RANK()`, `ROW_NUMBER()`
- التجميع: `SUM()`, `AVG()`, `COUNT()`, `MIN()`, `MAX()`
- الإحصاء: `FIRST_VALUE()`, `LAST_VALUE()`, `LAG()`, `LEAD()`

--

- **Full Text Search - البحث النصي المتقدم**

- *الغرض: بحث نصي متقدم في النصوص الطويلة*

- *المشكلة التي تحلها:*
  - *مشكلة LIKE:*

    ```sql
    -- ❌ بطيء وغير دقيق
    SELECT * FROM articles 
    WHERE content LIKE '%mysql%' OR content LIKE '%database%';
    ```

  - *حل Full Text Search:*

    ```sql
    -- ✅ سريع وذكي
    SELECT * FROM articles 
    WHERE MATCH(content) AGAINST('mysql database');
    ```

- *التطبيق العملي:*

*البيانات الأساسية:*

```sql
-- جدول المقالات
CREATE TABLE articles (
    id INT PRIMARY KEY AUTO_INCREMENT,
    title VARCHAR(200),
    content TEXT,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

INSERT INTO articles (title, content) VALUES
('تعلم MySQL', 'MySQL هي نظام إدارة قواعد بيانات علاقية مفتوح المصدر.'),
('برمجة Python', 'بايثون لغة برمجة عالية المستوى سهلة التعلم.'),
('قواعد البيانات', 'تعلم أساسيات قواعد البيانات والاستعلامات SQL.'),
('تطوير الويب', 'طور مواقع ويب باستخدام PHP و MySQL.');

-- إنشاء الفهرس النصي
CREATE FULLTEXT INDEX idx_content ON articles(content);
```

- المثال 1: البحث الأساسي

```sql
-- بحث عن كلمات "قواعد" و "بيانات"
SELECT title, content 
FROM articles 
WHERE MATCH(content) AGAINST('قواعد بيانات');
```

- المثال 2: البحث مع درجة الصلة (`Relevance`)

```sql
SELECT 
    title,
    content,
    MATCH(content) AGAINST('قواعد بيانات') as relevance_score
FROM articles 
WHERE MATCH(content) AGAINST('قواعد بيانات')
ORDER BY relevance_score DESC;
```

- المثال 3: `Boolean Mode` - بحث متقدم

```sql
-- (+: يجب وجود الكلمة)، (-: يجب عدم وجود الكلمة)
SELECT title, content
FROM articles 
WHERE MATCH(content) AGAINST('+MySQL -PHP' IN BOOLEAN MODE);
```

- *أنواع البحث في Full Text Search:*

1. `Natural Language Mode` (الافتراضي)

    ```sql
    -- بحث طبيعي يراعي تكرار الكلمات وأهميتها
    SELECT * FROM articles 
    WHERE MATCH(content) AGAINST('قواعد بيانات');
    ```

2. `Boolean Mode`

    ```sql
    -- تحكم كامل في البحث باستخدام مشغلات منطقية
    SELECT * FROM articles 
    WHERE MATCH(content) AGAINST('+MySQL +قواعد -Oracle' IN BOOLEAN MODE);
    ```

    - المشغلات:
       - `+` يجب وجود الكلمة
       - `-` يجب عدم وجود الكلمة  
       - `*` بحث جزئي (كلمات تبدأ بـ...)
       - `""` بحث عن عبارة كاملة

3. `Query Expansion`

    ```sql
    -- يوسع البحث تلقائياً ليشمل كلمات مشابهة
    SELECT * FROM articles 
    WHERE MATCH(content) AGAINST('database' WITH QUERY EXPANSION);
    ```

- *مقارنة شاملة:*

| Aspect | LIKE | Full Text Search |
|--------|------|------------------|
| **السرعة** | بطيء على بيانات كثيرة | سريع جداً |
| **الدقة** | مطابقة تامة فقط | بحث ذكي ومرن |
| **الترتيب** | لا يدعم ترتيب النتائج | يدعم ترتيب حسب الأهمية |
| **البحث الجزئي** | `%كلمة%` | بحث تلقائي عن الجذور |
| **البحث المتقدم** | محدود | Boolean operators |

- *مثال تطبيقي حقيقي:*

```sql
-- نظام مقالات مع بحث متقدم
SELECT 
    id,
    title,
    LEFT(content, 100) as content_preview,
    MATCH(content) AGAINST('قواعد بيانات MySQL') as relevance,
    created_at
FROM articles 
WHERE MATCH(content) AGAINST('قواعد بيانات MySQL' IN BOOLEAN MODE)
ORDER BY relevance DESC, created_at DESC
LIMIT 10;
```

--

- **🎯 ملخص أهم الاستعلامات:**

1. *✅ SELECT, INSERT, UPDATE, DELETE* - الأساسيات
2. *✅ JOINs* - ربط الجداول  
3. *✅ GROUP BY, HAVING* - التجميع
4. *✅ Subqueries, CTEs* - الاستعلامات المتداخلة
5. *✅ Transactions* - المعاملات
6. *✅ Indexes* - الفهارس
7. *✅ EXPLAIN* - تحليل الأداء
8. *✅ Prepared Statements* - الأمان

---

### PostgreSQL

---

#### Summary - الملخص

##### 1. الأساسيات (`Must Know`)

**المفاهيم الأساسية:**

- الفرق بين `SQL` و `NoSQL` ومتى تستخدم `PostgreSQL`
- تنصيب `PostgreSQL` محليًا
- أدوات الاتصال (`psql`, `pgAdmin`, `DBeaver`)

**العمليات الأساسية:**

```sql
-- إنشاء قاعدة بيانات
CREATE DATABASE myapp;

-- الجداول الأساسية
CREATE TABLE users (
    id SERIAL PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    email VARCHAR(255) UNIQUE NOT NULL,
    created_at TIMESTAMP DEFAULT NOW()
);

-- العمليات الأساسية (CRUD)
INSERT INTO users (name, email) VALUES ('أحمد', 'ahmed@example.com');
SELECT * FROM users WHERE id = 1;
UPDATE users SET name = 'محمد' WHERE id = 1;
DELETE FROM users WHERE id = 1;
```

##### 2. تصميم قواعد البيانات

**أنواع البيانات المهمة:**

- `SERIAL` / `BIGSERIAL` للـ Auto-increment
- `VARCHAR(n)` vs `TEXT`
- `INTEGER`, `BIGINT`, `NUMERIC` للأرقام
- `BOOLEAN`, `TIMESTAMP`, `DATE`
- `JSONB` للبيانات شبه المنظمة

**العلاقات:**

```sql
-- One-to-Many
CREATE TABLE posts (
    id SERIAL PRIMARY KEY,
    user_id INTEGER REFERENCES users(id),
    -- في جدول posts: user_id يجب ألا يكون unique لكي:
    -- يتمكن نفس المستخدم من إنشاء عدة منشورات
    -- لذا كل منشور جديد سيحمل نفس user_id الخاص بالمستخدم
    title VARCHAR(200) NOT NULL,
    content TEXT
);

-- Many-to-Many
CREATE TABLE user_roles (
    user_id INTEGER REFERENCES users(id),
    role_id INTEGER REFERENCES roles(id),
    PRIMARY KEY (user_id, role_id)
);
```

##### 3. الاستعلامات المتقدمة

**JOIN Operations:**

```sql
-- INNER JOIN
SELECT u.name, p.title 
FROM users u 
INNER JOIN posts p ON u.id = p.user_id;

-- LEFT JOIN
SELECT u.name, COUNT(p.id) as post_count
FROM users u 
LEFT JOIN posts p ON u.id = p.user_id
GROUP BY u.id, u.name;
```

**Aggregations:**

```sql
-- GROUP BY و HAVING
SELECT user_id, COUNT(*) as post_count
FROM posts 
GROUP BY user_id  -- عدد منشورات كل مستخدم
HAVING COUNT(*) > 5; -- المستخدمين الذين يملكون فوق 5 منشورات
```

**Window Functions:**

```sql
-- الترتيب والترقيم
SELECT name, salary,
    RANK() OVER (ORDER BY salary DESC) as rank
FROM employees;
```

##### 4. الأداء والتحسين

**الفهارس (Indexes):**

```sql
-- الفهرس الأساسي (تلقائي مع PRIMARY KEY)
-- فهرس على عمود مفرد
CREATE INDEX idx_users_email ON users(email);

-- فهرس مركب
CREATE INDEX idx_posts_user_date ON posts(user_id, created_at);

-- فهرس جزئي
CREATE INDEX idx_active_users ON users(email) WHERE is_active = true;
```

**تحليل الاستعلامات:**

```sql
-- EXPLAIN لتحليل أداء الاستعلام
EXPLAIN ANALYZE SELECT * FROM users WHERE email = 'test@example.com';
```

##### 5. الميزات المتقدمة للمطورين

**Stored Procedures and Functions:**

```sql
-- دالة تخزن بيانات المستخدم
CREATE OR REPLACE FUNCTION create_user(
    user_name VARCHAR, 
    user_email VARCHAR
) RETURNS INTEGER AS $$
DECLARE
    new_user_id INTEGER;
BEGIN
    INSERT INTO users (name, email) 
    VALUES (user_name, user_email)
    RETURNING id INTO new_user_id;
    
    RETURN new_user_id;
END;
$$ LANGUAGE plpgsql;
```

**Triggers:**

```sql
-- trigger لتسجيل التغييرات
CREATE TABLE audit_log (
    id SERIAL PRIMARY KEY,
    table_name VARCHAR(100),
    record_id INTEGER,
    action VARCHAR(10),
    changed_at TIMESTAMP DEFAULT NOW()
);

CREATE OR REPLACE FUNCTION log_changes()
RETURNS TRIGGER AS $$
BEGIN
    INSERT INTO audit_log (table_name, record_id, action)
    VALUES (TG_TABLE_NAME, COALESCE(NEW.id, OLD.id), TG_OP);
    RETURN NEW;
END;
$$ LANGUAGE plpgsql;
```

**Full-Text Search:**

```sql
-- البحث النصي المتقدم
ALTER TABLE posts ADD COLUMN search_vector tsvector;
CREATE INDEX idx_search ON posts USING gin(search_vector);

-- تحديث vector البحث
UPDATE posts SET search_vector = 
    to_tsvector('arabic', title || ' ' || content);
```

##### 6. الإدارة والأمان

**إدارة المستخدمين والصلاحيات:**

```sql
-- إنشاء مستخدم جديد
CREATE USER app_user WITH PASSWORD 'secure_password';

-- منح الصلاحيات
GRANT CONNECT ON DATABASE myapp TO app_user;
GRANT USAGE ON SCHEMA public TO app_user;
GRANT SELECT, INSERT, UPDATE ON users TO app_user;
```

**النسخ الاحتياطي:**

```bash
# نسخ احتياطي
pg_dump myapp > backup.sql

# استعادة
psql myapp < backup.sql
```

##### 7. التكامل مع لغات البرمجة

**مع Node.js:**

```javascript
// باستخدام pg library
const { Pool } = require('pg');
const pool = new Pool({
    user: 'app_user',
    host: 'localhost',
    database: 'myapp',
    password: 'password',
    port: 5432,
});

// استعلام
const result = await pool.query(
    'SELECT * FROM users WHERE id = $1', 
    [userId]
);
```

**مع Python:**

```python
import psycopg2

conn = psycopg2.connect(
    host="localhost",
    database="myapp",
    user="app_user",
    password="password"
)

cur = conn.cursor()
cur.execute("SELECT * FROM users WHERE id = %s", (user_id,))
```

##### 8. أفضل الممارسات

1. **تسمية الجداول والأعمدة:** استخدام `snake_case`
2. **استخدام المعلمات Parameterized Queries** لمنع `SQL Injection`
3. **النسخ الاحتياطي الدوري**
4. **مراقبة الأداء** باستخدام `pg_stat_statements`
5. **استخدام الاتصالات المجمعة** (`Connection Pooling`)

##### 9. مشروع عملي

**أنشئ تطبيق مدونة:**

- مستخدمين (`users`)
- مقالات (`posts`)
- تعليقات (`comments`)
- تصنيفات (`categories`)
- علاقات `many-to-many` بين المقالات والتصنيفات

##### 10.  مصادر التعلم

- **الوثائق الرسمية:** [postgresql.org/docs](https://www.postgresql.org/docs/)

- **ممارسة:** `HackerRank`, `LeetCode` للـ `SQL`

  - ما هو `HackerRank`, `LeetCode`؟
    - منصات تدريب برمجي - مثل صالات رياضية للبرمجة

    *HackerRank:*

    ```python
    # مثال سؤال: أوجد الرقم المكرر في المصفوفة
    def find_duplicate(nums):
    # أكتب الحل هنا
    pass
    # سيختبرون الحل بمدخلات مختلفة
    ```

    *LeetCode:*

    ```python
    # مثال سؤال: انسخ قائمة مرتبطة
    class Solution:
    def copyRandomList(self, head):
        # أكتب الحل
        return copied_head
    ```

    *لماذا يستخدمها المطورون؟:*

    - تحضير لمقابلات العمل
    - تحسين مهارات الخوارزميات
    - تحدي النفس مع مبرمجين آخرين

    - وكيف تتم ممارستهما للـ `SQL`

    **كيف تبدأ في كل منصة:**

    *1. HackerRank للـ SQL:*

    - الرابط: [hackerrank.com/domains/sql](https://www.hackerrank.com/domains/sql)

    *2. LeetCode للـ SQL:*

    - الرابط: [leetcode.com/studyplan/top-sql-50/](https://leetcode.com/studyplan/top-sql-50/)
    - رابط لقاعدة البيانات: [leetcode.com/problemset/database/](https://leetcode.com/problemset/database/)

- **كتب:** `"PostgreSQL Up and Running"`

--

#### Detail - التفاصيل

##### Phase 1: The Basics - المرحلة 1: الأساسيات

###### Basic Concepts and Installing - المفاهيم الأساسية والتثبيت

**ما هو PostgreSQL؟:**

- نظام إدارة قواعد بيانات علاقية (`RDBMS`) مفتوح المصدر
- يدعم `SQL` بالكامل ويتميز بالقوة والثبات
- ينافس `Oracle` و `MySQL` في المشاريع الكبيرة

**التثبيت:**

- رقم الإصدار الحالي (`18`)

```bash
# على Ubuntu
sudo apt-get update
sudo apt-get install postgresql postgresql-contrib

# على macOS
brew install postgresql

# على Windows
# حمل من موقع postgresql.org
```

**التأكد من نجاح التنزيل:**

- *ابحث على `SQL Shell` في التطبيقات وسيعرض الاعدادات ويطلب بالنهاية إدخال كلمة المرور التي تمت إضافتها عند التنزيل*

- *يمكن الآن كتابة الاستعلامات بسطر الأوامر مثلا:*

```shell
select version(); # الاستعلام عن الإصدار الحالي
```

- *الأفضل هو إضافة واجهة لكتابة الاستعلامات عليها*

**عرض الواجهة:**

1. ابحث على `pgAdmin 4` في التطبيقات

2. ستجد سيرفر جاهز مثل `PostgreSQL 18` أدخل فقط كلمة المرور

3. لإضافة سيرفر جديد:
   1. انقر بزر الماوس الأيمن على `Servers` ثم `Register` ثم `Server`
   2. اكتب اسمه في `General` مثلا: `localhost`
   3. اكتب عنوانه في `Connection\Address`: `localhost` أو `127.0.0.1`
   4. أدخل الباسوورد في `Connection\Password`
   5. لتفعيل السيرفر انقر بزر الماوس الأيمن عليه ثم `Connect Server`

4. لإضافة قاعدة بيانات انقر بزر الماوس الأيمن على السيرفر ثم `Create` ثم `Database` ثم أنشئ القاعدة

5. لكتابة الاستعلامات انقر بزر الماوس الأيمن على القاعدة المحددة ثم اختر `Query Tools`

###### Communication tools - أدوات الاتصال

**أدوات سطر الأوامر (psql):**

```sql
-- إضافة المحرك للمسار في النظام (في حالة استخدم سطر أوامر آخر)
"C:\Program Files\PostgreSQL\18\bin\psql.exe" -U postgres

-- الدخول إلى قاعدة البيانات
psql -U username -d database_name -h host

-- الأوامر الأساسية في psql
\l              -- عرض قواعد البيانات
\c database_name -- الانتقال إلى قاعدة بيانات
\dt             -- عرض الجداول
\d table_name   -- وصف الجدول
\?              -- مساعدة الأوامر
\h              -- مساعدة SQL
-- SHIFT + Q    -- الخروج إن لم يتوقف التنفيذ
```

**أدوات واجهة رسومية:**

- **pgAdmin**: الأداة الرسمية
- **DBeaver**: أداة متعددة قواعد البيانات
- **DataGrip**: من `JetBrains` (مدفوعة)

###### Creating and Managing Databases - إنشاء وإدارة قواعد البيانات

```sql
-- عرض القاعدة المتصل بها
SELECT current_database();

-- إنشاء قاعدة بيانات
CREATE DATABASE company;

-- للاتصال بقاعدة البيانات انقر بزر الماوس الأيمن على Databases بالشريط الجانبي ثم Refresh ثم أنقر على القاعدة ثم انقر بزر الماوس الأيمن عليها ثم Query Tool

-- إنشاء جداول
CREATE TABLE employees (
    id SERIAL PRIMARY KEY,
    first_name VARCHAR(50) NOT NULL,
    last_name VARCHAR(50) NOT NULL,
    email VARCHAR(100) UNIQUE,
    salary DECIMAL(10,2),
    hire_date DATE DEFAULT CURRENT_DATE,
    department_id INTEGER
);

-- عرض الجداول
SELECT * FROM employees
```

###### Basic Operations (CRUD) - العمليات الأساسية

```sql
-- الإدراج (Create)
-- استخدم ' للنصوص/السلاسل النصية
-- استخدم " فقط لأسماء الجداول/الأعمدة (عند الحاجة)
INSERT INTO employees ("first_name", "last_name", "email", salary, department_id)
VALUES 
('أحمد', 'علي', 'ahmed.ali@company.com', 5000.00, 1),
('فاطمة', 'محمد', 'fatima.mohamed@company.com', 6000.00, 2);

-- القراءة (Read)
SELECT * FROM employees;
SELECT first_name, last_name, salary FROM employees;
SELECT * FROM employees WHERE salary > 5500;

-- التحديث (Update)
UPDATE employees 
SET salary = salary * 1.1 
WHERE department_id = 1;

-- الحذف (Delete)
DELETE FROM employees WHERE id = 1;
```

###### Data Types and Constraints - أنواع البيانات والقيود

**أنواع البيانات الأساسية:**

*التسلسل التلقائي (`Auto-increment`):*

- `PostgreSQL` لا يدعم الكلمة المفتاحية `AUTO_INCREMENT` للزيادة التلقائية كما في `MySQL` لذا يوجد بدائل:

1. `SERIAL` / `BIGSERIAL` (اختصار ينشئ `sequence` ويضع `DEFAULT nextval`)

   - `SERIAL`: يولد أرقام صحيحة تزداد تلقائياً (`4 bytes`، 1 to 2,147,483,647) للجداول الصغيرة والمتوسطة

   - `BIGSERIAL`:  نفس `SERIAL` لكن بمدى أكبر (`8 bytes`، 1 to 9,223,372,036,854,775,807) للجداول الكبيرة جداً

    ```sql
    CREATE TABLE users1 (
        id SERIAL PRIMARY KEY,
        name TEXT
    );
    ```

2. `IDENTITY` (تابع لمعيار `SQL`، متاح منذ `PostgreSQL 10`)

    ```sql
    CREATE TABLE users2 (
        id INT GENERATED ALWAYS AS IDENTITY PRIMARY KEY,
        name TEXT
    );
    ```

3. إنشاء `sequence` يدوياً واستخدام `nextval()`

    ```sql
    CREATE SEQUENCE users_id_seq;
    CREATE TABLE users3 (
        id INT DEFAULT nextval('users_id_seq') PRIMARY KEY,
        name TEXT
    );
    ```

- إدراج البيانات:

```sql
INSERT INTO users1 (name) VALUES ('a'), ('b'), ('c');
INSERT INTO users2 (name) VALUES ('a'), ('b'), ('c');
INSERT INTO users3 (name) VALUES ('a'), ('b'), ('c');

-- للحصول على معرف السطر المدرج استخدم RETURNING:
INSERT INTO users1 (name) VALUES ('أحمد') RETURNING id;  -- 4
INSERT INTO users2 (name) VALUES ('أحمد') RETURNING id;  -- 4
INSERT INTO users3 (name) VALUES ('أحمد') RETURNING id;  -- 4
```

*النصوص:*

- `VARCHAR(n)`, `CHARACTER VARYING(n)`: نص بطول محدد، يحفظ المساحة (مناسب للبريد الإلكتروني، الأسماء)

- `TEXT`: نص طويل بطول غير محدود (مناسب للمحتوى الطويل، المقالات)

- `CHAR(s)`, `CHARACTER(s)`: نص بطول ثابت يُخزن دائماً عدد حروف ثابت، وإذا أدخلت أقل تُملأ المسافات البيضاء إلى اليمين يعني يضيف فراغات في النهاية تكمل العدد وقد يتم تجاهلها

*الأرقام:*

- `INTEGER`: عدد صحيح (`4 bytes`) -2147483648 to +2147483647

- `BIGINT`: عدد صحيح كبير جداً

- `DECIMAL(p,s)`, `NUMERIC(p,s)`: عدد عشري

  - هما متطابقان تماماً في `PostgreSQL`
  - دقة عالية جداً (`arbitrary precision`)
  - مثالي للعمليات المالية والحسابات الدقيقة
  - يأخذان معاملين: `NUMERIC(precision, scale)`

  - `p` = `precision` = إجمالي عدد الأرقام كلها (قبل وبعد الفاصلة).
  - `s` = `scale` = عدد الأرقام بعد الفاصلة العشرية.

  - مثال: `DECIMAL(10,2)`
    - الإجمالي = `10` رقم.
    - بعد الفاصلة = `2` رقم.
    - إذن أقصى أرقام قبل الفاصلة = `10 - 2 = 8` رقم.
    - أعلى قيمة موجبة ممكنة ≈ `99999999.99`
  
  - نقاط قصيرة:
    - إذا حُددت قيمة لها أكثر من `s` منازل عشرية تُقرب إلى `scale` المحدد.
    - إذا تجاوز مجموع الأرقام `precision` تحصل على خطأ (`numeric field overflow`).
    - إذا لم تحدد (`p`,`s`) فـ `NUMERIC`/`DECIMAL` في `PostgreSQL` يعمل بدقة غير محدودة تقريباً (`arbitrary precision`).

- `REAL`: عدد عائم

  - يخزن ~6 أرقام عشرية بدقة (6 منازل عشرية)
  - دقة محدودة للخانات الكثيرة
  - أسرع في المعالجة من `NUMERIC`
  - مناسب للقياسات والقيم التقريبية، القياسات الفيزيائية، التقييمات
  - حجم تخزين ثابت (4 bytes)

  ```sql
  SELECT 12345678.99::DECIMAL(10,2); -- OK
  SELECT 123456789.99::DECIMAL(10,2); -- numeric field overflow
  SELECT 1.2345::DECIMAL(5,2);        -- يُقرب إلى 1.23

  CREATE TABLE price_comparison (
      id SERIAL PRIMARY KEY,
      exact_price NUMERIC(10,2),
      approx_price REAL,
      description VARCHAR(50)
  );
  INSERT INTO price_comparison (exact_price, approx_price, description) VALUES
    (123.45, 123.45, 'نفس القيمة'),
    (123.456789, 123.456789, 'NUMERIC سيقرب القيمة');
  ```

*التاريخ والوقت:*

- `DATE`: تاريخ فقط

- `TIMESTAMP`: تاريخ + وقت

- `TIMESTAMPTZ`: مع التوقيت الزمني

- الفرق بين `TIMESTAMP` و `TIMESTAMPTZ`
  - `TIMESTAMP` (بدون منطقة زمنية)
    - يخزن قيمة تاريخ/وقت حرفياً كما دخلت (لا يحتفظ بمعلومة المنطقة).
    - لا يتم تحويله عند العرض — يظل كما هو.
    - مناسب للأوقات المحلية الثابتة (مثل تاريخ الميلاد، مواعيد محلية لا تعني لحظة عالمية).

  - `TIMESTAMPTZ` (`TIMESTAMP WITH TIME ZONE`)
    - يخزن "لحظة زمنية" واحدة (يُخزّن داخلياً كـ `UTC`).
    - عند الإدخال: إذا أعطيت مع تعويض زمني (+03) يُحوّل إلى `UTC` ؛ إذا أعطيت بدون تعويض يُفهم بحسب `TimeZone` للجلسة ثم يُحوّل إلى `UTC`.
    - عند العرض: يُحوّل من `UTC` إلى `TimeZone` الجلسة ويعرض مع إزاحة.
    - مناسب لأحداث/سجلات زمنية (`logs`، تواقيت الأحداث) حيث تهم اللحظة المطلقة.

  - أمثلة عملية:

  ```sql
  CREATE TABLE times (t_plain TIMESTAMP, t_z TIMESTAMPTZ);

  INSERT INTO times VALUES
    ('2025-11-07 10:00', '2025-11-07 10:00+03'); -- الأول: حرفي، الثاني: مع إزاحة

  SET TIME ZONE 'UTC';
  SELECT t_plain, t_z FROM times;
  -- t_plain -> 2025-11-07 10:00
  -- t_z    -> 2025-11-07 07:00+00  (محول إلى UTC عند الإدخال ثم معروض بـ UTC)

  SET TIME ZONE 'Asia/Riyadh'; -- +03
  SELECT t_plain, t_z FROM times;
  -- t_plain -> 2025-11-07 10:00
  -- t_z    -> 2025-11-07 10:00+03  (معروض بالمنطقة الجلسة)
  ```

  - تحويلات مفيدة (`AT TIME ZONE`):

  ```sql
  -- يُعامل timestamp كقيميّة محلية في المنطقة ثم يُرجع timestamptz
  SELECT '2025-11-07 10:00'::timestamp AT TIME ZONE 'Europe/Berlin';  -- -> timestamptz

  -- يُحوّل timestamptz إلى توقيت محلي في المنطقة ويُرجع timestamp (بلا منطقة)
  SELECT '2025-11-07 10:00+01'::timestamptz AT TIME ZONE 'UTC';      -- -> timestamp
  ```

  - نصيحة عملية:
    - سجّل الأحداث الزمنية باستخدام `TIMESTAMPTZ`.
    - احتفظ بـ `TIMESTAMP` بدون `tz` للقيم المحلية التي لا تحتاج تحويل (`birth_date`، `opening_hours`).

*منطقية:*

- `BOOLEAN`: true/false

*خاصة بـ PostgreSQL:*

- `TEXT[]`: مصفوفة

  - `TEXT[]` مقابل `TEXT`

    - `text` = سلسلة نصية واحدة (مقدار واحد).
    - `text[]` = مصفوفة من سلاسل نصية (عدة قيم في خلية واحدة).

  - أمثلة إدخال واستعلام:

  ```sql
  CREATE TABLE t_array (
    id SERIAL PRIMARY KEY,
    tags TEXT[]  -- حقل مصفوفة نصية
  );

  INSERT INTO t_array (tags) VALUES
    (ARRAY['sql','python']),       -- طريقة ARRAY
    ('{"html","css"}'::text[]);    -- أو literal

  -- عناصر تحتوي على 'sql'؟
  SELECT * FROM t_array WHERE tags @> ARRAY['sql']::text[];  -- contains
  -- أو باستخدام ANY:
  SELECT * FROM t_array WHERE 'sql' = ANY(tags);

  -- فك عناصر المصفوفة صفّاً صفّاً:
  SELECT id, unnest(tags) AS tag FROM t_array;
  ```

- `JSONB`: البيانات شبه المنظمة، يخزن `JSON` مع إمكانية البحث والفهرسة

    ```sql
    CREATE TABLE json_examples (
        id SERIAL PRIMARY KEY,
        data JSONB
    );

    INSERT INTO json_examples (data) VALUES 
    ('{"name": "أحمد", "skills": ["SQL", "Python"]}');

    -- 1) بحث حسب اسم
    SELECT * FROM json_examples WHERE data->>'name' = 'أحمد';

    -- 2) تحقق أن المصفوفة skills تحتوي 'SQL' (طريقتان)
    SELECT * FROM json_examples WHERE data->'skills' ? 'SQL';                    -- ? يعمل على jsonb arrays/objects
    SELECT * FROM json_examples WHERE data @> '{"skills":["SQL"]}'::jsonb;      -- containment

    -- 3) فك عناصر الـ skills والتحقق
    SELECT id, jsonb_array_elements_text(data->'skills') AS skill
    FROM json_examples;

    -- لتحسين الأداء: فهرس GIN على JSONB
    CREATE INDEX idx_json_examples_data_gin ON json_examples USING GIN (data);
    ```

*مثال كامل:*

```sql
CREATE TABLE data_types_demo (

    -- التسلسل التلقائي (`Auto-increment`)
    id SERIAL PRIMARY KEY,
    big_id BIGSERIAL PRIMARY KEY

    -- النصوص
    name VARCHAR(100),
    description TEXT,
    code CHAR(5),

    -- الأرقام
    age INTEGER,
    population BIGINT,
    price1 DECIMAL(10,2),
    price2 NUMERIC(10,2),
    rating REAL,

    -- التاريخ والوقت
    birth_date DATE,
    created_at TIMESTAMP,
    updated_at TIMESTAMPTZ,
    
    -- منطقية
    is_active BOOLEAN,
    
    -- خاصة بـ PostgreSQL
    tags TEXT[],
    metadata JSONB
);
```

**القيود (Constraints):**

```sql
CREATE TABLE products (
    id SERIAL PRIMARY KEY,                    -- مفتاح رئيسي
    name VARCHAR(100) NOT NULL,              -- لا يقبل NULL
    sku VARCHAR(50) UNIQUE,                  -- فريد
    price DECIMAL(10,2) CHECK (price > 0),   -- شرط
    category_id INTEGER REFERENCES categories(id) -- مفتاح خارجي (يجب أن يكون جدول categories موجودا)
);
```

##### Phase 2: Advanced Queries - المرحلة 2: الاستعلامات المتقدمة

###### WHERE وترتيب النتائج

```sql
-- عوامل المقارنة
SELECT * FROM employees WHERE salary > 5000;
SELECT * FROM employees WHERE hire_date >= '2023-01-01';

-- BETWEEN و IN
SELECT * FROM employees WHERE salary BETWEEN 4000 AND 7000;
SELECT * FROM employees WHERE department_id IN (1, 3, 5);

-- LIKE للبحث النصي
SELECT * FROM employees WHERE first_name LIKE 'أح%';  -- يبدأ بأح
SELECT * FROM employees WHERE last_name LIKE '%محمد%'; -- يحتوي على محمد

-- ORDER BY للترتيب
SELECT * FROM employees ORDER BY salary DESC;
SELECT * FROM employees ORDER BY last_name ASC, first_name ASC;

-- LIMIT و OFFSET
SELECT * FROM employees ORDER BY salary DESC LIMIT 5;
SELECT * FROM employees ORDER BY hire_date LIMIT 10 OFFSET 20; -- للترقيم
```

###### Built-in Functions - الدوال المـدمجة

**الدوال الأساسية:**

*String Functions - دوال النصوص:*

تُستخدم للتعامل مع النصوص في `SQL Queries` وعمليات البحث والفصل.

| الدالة                          | الوصف                              | مثال                                     |
| ------------------------------- | ---------------------------------- | ---------------------------------------- |
| `LOWER(text)`                   | تحويل النص إلى حروف صغيرة          | `LOWER('HELLO') → 'hello'`               |
| `UPPER(text)`                   | تحويل النص إلى حروف كبيرة          | `UPPER('hello') → 'HELLO'`               |
| `INITCAP(text)`                 | جعل أول حرف من كل كلمة كبير        | `INITCAP('hello world') → 'Hello World'` |
| `LENGTH(text)`                  | عدد الحروف في النص                 | `LENGTH('Hello') → 5`                    |
| `TRIM(text)`                    | إزالة الفراغات من البداية والنهاية | `TRIM('  hi  ') → 'hi'`                  |
| `SUBSTRING(text, from, for)`    | استخراج جزء من النص                | `SUBSTRING('abcdef', 2, 3) → 'bcd'`      |
| `CONCAT(a, b, ...)`             | دمج النصوص                         | `CONCAT('a', 'b') → 'ab'`                |
| `POSITION(substring IN string)` | موضع بداية جزء داخل النص           | `POSITION('a' IN 'data') → 2`            |
| `REPLACE(text, from, to)`       | استبدال جزء بآخر                   | `REPLACE('abc', 'a', 'z') → 'zbc'`       |

*Numeric Functions - دوال الأرقام:*

| الدالة                        | الوصف                        | مثال                       |
| ----------------------------- | ---------------------------- | -------------------------- |
| `ROUND(num, decimals)`        | التقريب لعدد معين من الخانات | `ROUND(3.14159, 2) → 3.14` |
| `CEIL(num)` أو `CEILING(num)` | التقريب للأعلى               | `CEIL(4.2) → 5`            |
| `FLOOR(num)`                  | التقريب للأسفل               | `FLOOR(4.8) → 4`           |
| `ABS(num)`                    | القيمة المطلقة               | `ABS(-5) → 5`              |
| `POWER(x, y)`                 | القوة (أس)                   | `POWER(2, 3) → 8`          |
| `RANDOM()`                    | رقم عشوائي بين 0 و1          | `RANDOM() → 0.345`         |
| `PI()`                        | قيمة π                       | `PI() → 3.14159`           |

*Date & Time Functions - دوال التاريخ والوقت:*

| الدالة                      | الوصف                             | مثال                                          |
| --------------------------- | --------------------------------- | --------------------------------------------- |
| `NOW()`                     | التاريخ والوقت الحاليان           | `NOW() → 2025-11-07 14:23:00`                 |
| `CURRENT_DATE`              | التاريخ فقط                       | `CURRENT_DATE → 2025-11-07`                   |
| `CURRENT_TIME`              | الوقت فقط                         | `CURRENT_TIME → 14:23:00`                     |
| `AGE(timestamp, timestamp)` | الفرق بين تاريخين                 | `AGE('2025-01-01', '2024-01-01') → 1 year`    |
| `EXTRACT(field FROM date)`  | استخراج جزء (مثل السنة، الشهر...) | `EXTRACT(YEAR FROM NOW()) → 2025`             |
| `DATE_PART(field, date)`    | مثل EXTRACT                       | `DATE_PART('month', NOW()) → 11`              |
| `TO_CHAR(date, format)`     | تنسيق التاريخ كنص                 | `TO_CHAR(NOW(), 'YYYY-MM-DD') → '2025-11-07'` |

*Conversion Functions - دوال التحويل:*

| الدالة                       | الوصف              | مثال                                                     |
| ---------------------------- | ------------------ | -------------------------------------------------------- |
| `CAST(value AS type)`        | تحويل نوع البيانات | `CAST('10' AS INTEGER) → 10`                             |
| `TO_NUMBER(text, format)`    | تحويل نص إلى رقم   | `TO_NUMBER('1,200', '9,999') → 1200`                     |
| `TO_DATE(text, format)`      | تحويل نص إلى تاريخ | `TO_DATE('07-11-2025', 'DD-MM-YYYY')`                    |
| `TO_TIMESTAMP(text, format)` | نص إلى طابع زمني   | `TO_TIMESTAMP('2025-11-07 12:00', 'YYYY-MM-DD HH24:MI')` |

- ملاحظات حول `TO_NUMBER(text, format)`:

  - هي دالة تتعامل مع قيم نصية (`Strings`) تحتوي على أرقام منسقة وتحتاج لتحويلها إلى أرقام رقمية (`Numeric`) لتستطيع إجراء عمليات حسابية عليها فوظيفتها تحويل نص (`text`) يمثل رقمًا منسقًا إلى قيمة رقمية (`numeric`) حقيقية.
  - تخيل أن لديك بيانات أرقام مخزنة كنصوص مثل:

    ```text
    '1,200.50'
    '$3,000'
    '12.5%'
    ```

    > لا يمكنك جمعها أو حسابها مباشرة لأنها ليست أرقامًا، بل نصوص تحتوي على رموز مثل الفواصل أو علامة الدولار أو النسبة المئوية فهنا يأتي دور الدالة
  
  - الصيغة العامة:

  ```sql
  TO_NUMBER('text', 'format')
  ```

  - `text`: هو النص الذي يحتوي على الرقم.
  - `format`: يوضح شكل الرقم داخل النص حتى يعرف `PostgreSQL` كيف يفسّره.

  - أمثلة عملية:

    ```sql
    SELECT TO_NUMBER('1,200.50', '9,999.99');  -- 1200.50
    -- '1,200.50' هو نص.
    -- النمط '9,999.99' يخبر PostgreSQL أن:
    -- هناك فاصلة بين الآلاف.
    -- ويوجد جزء عشري بعد النقطة.

    SELECT TO_NUMBER('$3,000', '$9,999');  -- 3000
    -- `$9,999` يعني أن الرمز `$` موجود في النص.
    -- PostgreSQL يتجاهله أثناء التحويل ويحوّله إلى رقم.

    SELECT TO_NUMBER('12.5%', '99.9%');  -- 12.5

    SELECT TO_NUMBER('007', '999');  -- 7
    -- لأن الأصفار في النمط لا تُعتبر جزءًا من القيمة الرقمية النهائية.
    ```

  - ملاحظات مهمة:
    - إن لم يتطابق النمط مع النص، سيُرجع `PostgreSQL` خطأ.
    - هذه الدالة لا تقبل الفراغات أو رموز غير مذكورة في النمط.
    - تُستخدم غالبًا مع استيراد البيانات من `CSV` أو `Excel`، حيث تكون الأرقام منسقة كـ `"1,234.56"` أو `"£5,000"`.
  
  - خلاصة:

    | الحالة                     | النتيجة                       |
    | -------------------------- | ----------------------------- |
    | نص يحتوي على فواصل أو رموز | استخدم `TO_NUMBER()`          |
    | نص بسيط مثل `'123'`        | يكفي `CAST('123' AS INTEGER)` |

  - معنى الرقم `9` في التنسيق يعني مكان يمكن أن يحتوي على رقم (0–9)، وإذا لم يوجد رقم يُترك فارغًا.
  - مثلاً:

  ```sql
  SELECT TO_NUMBER('123', '9999');  -- 123
  -- لأن النص 123 يناسب النمط 9999 (4 أماكن رقمية).
  -- ولو كان النص 0123 فسيتم تحويله إلى نفس القيمة الرقمية 123.
  ```

  - الرموز الأخرى التي يمكن استخدامها:

    | الرمز | المعنى                                       | المثال                                            | النتيجة |
    | ----- | -------------------------------------------- | ------------------------------------------------- | ------- |
    | `9`   | خانة رقمية اختيارية                          | `TO_NUMBER('123', '9999')`                        | 123     |
    | `0`   | خانة رقمية إلزامية (تظهر الأصفار)            | `TO_CHAR(5, '000')` → `'005'` *(معكوس TO_NUMBER)* |         |
    | `.`   | الفاصل العشري                                | `TO_NUMBER('12.5', '99.9')` → 12.5                |         |
    | `,`   | فاصل الآلاف                                  | `TO_NUMBER('1,200', '9,999')` → 1200              |         |
    | `$`   | رمز الدولار                                  | `TO_NUMBER('$3,000', '$9,999')` → 3000            |         |
    | `L`   | رمز العملة المحلية (حسب الإعدادات الإقليمية) | `TO_NUMBER('£500', 'L999')` → 500                 |         |
    | `%`   | نسبة مئوية                                   | `TO_NUMBER('25%', '99%')` → 25                    |         |

  - ما الذي يحدث لو استخدمت رمزًا غير مناسب؟

  - مثلاً:

    ```sql
    SELECT TO_NUMBER('1,200', '9999');  -- 120
    ```

    - ❌ سيُنتج `120`، لأن النمط `'9999'` لا يحتوي على فاصلة، بينما النص يحتوي عليها.

    - يجب أن تكتب:

    ```sql
    SELECT TO_NUMBER('1,200', '9,999'); -- 1200
    -- الآن PostgreSQL يفهم أن الفاصلة جزء من التنسيق.
    ```

  - خلاصة بسيطة

  | الحالة              | النمط المقترح | مثال          |
  | ------------------- | ------------- | ------------- |
  | رقم عادي بدون فواصل | `'999'`       | `'123'`       |
  | رقم بفاصلة          | `'9,999'`     | `'1,234'`     |
  | رقم عشري            | `'9,999.99'`  | `'1,234.56'`  |
  | رقم مع عملة         | `'$9,999.99'` | `'$1,234.56'` |
  | نسبة مئوية          | `'99%'`       | `'25%'`       |

  - عند استخدام:

    ```sql
    TO_NUMBER('1,200', '9,999')
    ```

  - فهو لا يقرأ الرقم الثاني كقيمة، بل كقناع (`mask`) يوضح شكل الرقم في النص، يعني:

    - كل `9` → مكان يمكن أن يحتوي على رقم من 0 إلى 9
    - الفاصلة `,` → حرف فاصل للآلاف
    - النقطة `.` → فاصل عشري
    - الرموز الأخرى مثل `$`, `%` يمكن استخدامها لكن ليس أي رقم آخر
  
  - لذلك عند كتابة:

    ```sql
    SELECT TO_NUMBER('1,200', '8,6708');
    ```

  - ❌ هذا غير صحيح لأن `PostgreSQL` يقرأ الـ `8` و `6` و `7` و `0` كرموز غير مفهومة في القناع. فهو يتوقع شيئًا مثل:

    ```sql
    '9,999'
    '9,999.99'
    '$9,999'
    ```

    - وليس `'8,6708'` — لأن هذه ليست رموز تنسيق معروفة.

  - القاعدة الذهبية

    > داخل نمط التنسيق (`format`)،
    > لا يُستخدم الرقم للدلالة على قيم حقيقية،
    > بل يُستخدم الرمز 9 أو 0 فقط لتحديد خانات الأرقام.
    > الأرقام الأخرى (1، 2، 3، 4...) لا معنى لها، ولهذا سيعطي `PostgreSQL` صفر بدل النتيجة الصحيحة.

  - لذا يجب أن يكون رقم التنسيق هو 9 أو 0 في دالة `TO_NUMBER()` لأن `PostgreSQL` لا يقرأها كأرقام حقيقية،
بل كرموز (`placeholders`) تمثل خانات الأرقام داخل النص.

  - التوضيح النهائي السريع:

    - الرقم 9 → يعني هنا خانة رقمية ممكن يكون فيها أي رقم 0–9.
    - الرقم 0 → يعني خانة رقمية إلزامية (تُظهر الأصفار لو لم يوجد رقم).
    - أما أي رقم آخر (مثل 8 أو 7 أو 3...) → ❌ `PostgreSQL` لا يفهمه كرمز تنسيق، بل كحرف غير معروف داخل القناع، وبالتالي النتيجة تكون 0 أو خطأ.

*Aggregate Functions - دوال التجميع:*

تُستخدم مع `GROUP BY`.

| الدالة        | الوصف       | مثال             |
| ------------- | ----------- | ---------------- |
| `COUNT(*)`    | عدد الصفوف  | `COUNT(*) → 100` |
| `SUM(column)` | مجموع القيم | `SUM(price)`     |
| `AVG(column)` | المتوسط     | `AVG(age)`       |
| `MIN(column)` | أصغر قيمة   | `MIN(salary)`    |
| `MAX(column)` | أكبر قيمة   | `MAX(salary)`    |

*Conditional Functions - دوال منطقية وشَرطية:*

| الدالة                    | الوصف                | مثال                                          |
| ------------------------- | -------------------- | --------------------------------------------- |
| `COALESCE(a, b, c, ...)`  | أول قيمة غير NULL    | `COALESCE(NULL, NULL, 5) → 5`                 |
| `NULLIF(a, b)`            | ترجع NULL إذا تساويا | `NULLIF(5, 5) → NULL`                         |
| `CASE WHEN THEN ELSE END` | شرط متعدد            | `CASE WHEN x > 10 THEN 'high' ELSE 'low' END` |

*دوال JSON (مهمة جدًا في الـ APIs):*

| الدالة                               | الوصف                 | مثال                                          |
| ------------------------------------ | --------------------- | --------------------------------------------- |
| `TO_JSON(any)`                       | تحويل قيمة إلى JSON   | `TO_JSON(ARRAY[1,2,3]) → [1,2,3]`             |
| `JSON_BUILD_OBJECT(key, value, ...)` | إنشاء كائن JSON       | `JSON_BUILD_OBJECT('id', 1, 'name', 'Ahmed')` |
| `JSON_EXTRACT_PATH(json, key)`       | استخراج قيمة من JSON  | `JSON_EXTRACT_PATH('{"a":1}', 'a') → 1`       |
| `JSONB_SET(jsonb, path, new_value)`  | تعديل قيمة داخل JSONB | —                                             |

*Row & Table Functions - دوال صفوف وجداول:*

| الدالة                                  | الوصف                         |
| --------------------------------------- | ----------------------------- |
| `UNNEST(array)`                         | تفكيك مصفوفة إلى صفوف         |
| `GENERATE_SERIES(start, stop [, step])` | توليد أرقام أو تواريخ متتابعة |
| `ARRAY_AGG(column)`                     | تجميع قيم في مصفوفة           |

*System Information Functions - دوال معلومات النظام: Sequence Manipulation Functions - دوال معالجة التسلسل:*

- الدوال الرئيسية للتسلسلات:

```sql
-- الحصول على القيمة التالية
SELECT nextval('sequence_name'); 

-- الحصول على القيمة الحالية (في نفس الجلسة)
SELECT currval('sequence_name');

-- تعيين قيمة للتسلسل
SELECT setval('sequence_name', 100);

-- الحصول على آخر قيمة مُعينة (عبر جميع الجلسات)
SELECT lastval();
```

- `currval`: هي دالة تُرجع القيمة الحالية (`current value`) لتسلسل (`sequence`) محدد في نفس الجلسة.

- `'table_column_seq'`: اسم التسلسل الذي نريد قيمته الحالية

- يجب أن يكون قد تم استخدام `nextval` على هذا التسلسل في نفس الجلسة قبل استخدام `currval`

- مثال كامل:

```sql
-- إنشاء الجداول والتسلسل
CREATE TABLE orders (
    id SERIAL PRIMARY KEY,
    order_date DATE
);

CREATE TABLE order_items (
    id SERIAL PRIMARY KEY,
    order_id INTEGER REFERENCES orders(id),
    product_id INTEGER,
    quantity INTEGER
);

-- إدخال الطلب (يستخدم nextval تلقائياً)
INSERT INTO orders (order_date) VALUES (CURRENT_DATE);

-- إدخال تفاصيل الطلب (يستخدم currval لنفس معرف الطلب)
INSERT INTO order_items (order_id, product_id, quantity) 
VALUES (currval('orders_id_seq'), 1, 2);
```

- ملاحظات مهمة
  - يجب استخدام `nextval` قبل `currval`
  - `currval` تعمل فقط في نفس الجلسة

- الفكرة الأساسية لـ `currval`

  - `currval` لا يجلب سجلات من جدول آخر، بل يعيد القيمة الحالية للتسلسل (`sequence`) فقط.

- مثال للتوضيح:

```sql
CREATE TABLE test1 (test1_id SERIAL PRIMARY KEY);
CREATE TABLE test2 (test2_id INTEGER REFERENCES test1(test1_id));

INSERT INTO test1 VALUES (1);    -- test1_id = 1
INSERT INTO test1 VALUES (10);   -- test1_id = 10
INSERT INTO test2 VALUES (currval('test1_test1_id_seq')); -- سترجع 10
```

- ما الذي يحدث هنا؟:

  1. عندما تستخدم `SERIAL`، يتم إنشاء تسلسل تلقائيًا باسم `test1_test1_id_seq`
  2. `INSERT INTO test1 VALUES (10)` تستخدم `nextval` تلقائيًا وتجعل القيمة الحالية = 10
  3. `currval('test1_test1_id_seq')` ترجع *10* - آخر قيمة استخدمها التسلسل

- السيناريو الشائع للاستخدام

```sql
-- إدخال طلب رئيسي
INSERT INTO orders (order_date) VALUES (CURRENT_DATE); 
-- التسلسل orders_id_seq أصبحت قيمته الحالية = X

-- إدخال تفاصيل تستخدم نفس معرف الطلب
INSERT INTO order_items (order_id, product_id, quantity) 
VALUES (currval('orders_id_seq'), 1, 2);
-- هنا currval ترجع X بدون حاجة لمعرفته مسبقاً
```

- يعني `currval` مجرد طريقة للحصول على آخر قيمة تسلسل

تستخدم `currval` عندما تريد إدخال بيانات في جدولين مرتبطين، وتحتاج استخدام نفس `ID` الذي تم إنشاؤه تلقائيًا في الجدول الرئيسي.

- بديل أفضل: استخدم `RETURNING`

```sql
WITH new_order AS (
    INSERT INTO orders (order_date) 
    VALUES (CURRENT_DATE) 
    RETURNING id
)
INSERT INTO order_items (order_id, product_id, quantity)
SELECT id, 1, 2 FROM new_order;
```

*ملاحظات:*

- استخدم `COALESCE` دائمًا لتفادي القيم `NULL` في النتائج.
- دوال `TO_CHAR` و `EXTRACT` مهمة جدًا في تقارير الزمن والإحصائيات.
- دوال `JSON` أصبحت أساسية في `PostgreSQL` منذ الإصدار 9.4 (وتحسنت كثيرًا في 15–18).
- راجع دائمًا الصفحة الرسمية:
  🔗 [PostgreSQL Functions and Operators – v18](https://www.postgresql.org/docs/18/functions.html)

###### Aggregations Functions - دوال التجميع

**GROUP BY:** يُستخدم لتجميع البيانات بناءً على عمود معين وحساب إحصائيات مثل العد والمتوسط.

- مثال عدد الموظفين ومتوسط الرواتب حسب كل قسم:

```sql
SELECT 
    department_id,  -- يتم تجميع البيانات حسب هذا العمود (عمود القسم)، مما يعني أن كل مجموعة تمثل قسمًا واحدًا.
    COUNT(*) as employee_count,  -- يحسب عدد الموظفين في كل قسم.
    AVG(salary) as avg_salary  -- يحسب متوسط الرواتب للموظفين في كل قسم.
FROM employees
GROUP BY department_id;  -- يقوم بتجميع النتائج بناءً على قيم department_id، مما ينتج عنه صف واحد لكل قسم مع إحصائياته.
```

**HAVING:** شرط على المجموعات: يُستخدم لتصفية النتائج بعد التجميع، حيث يمكن تطبيق شروط على النتائج المجمعة.

```sql
SELECT 
    department_id,  -- يتم تجميع البيانات حسب القسم
    COUNT(*) as employee_count  -- يحسب عدد الموظفين في كل قسم.
FROM employees
GROUP BY department_id  -- يقوم بتجميع النتائج بناءً على قيم department_id.
HAVING COUNT(*) > 5;  -- يحدد شرطًا على المجموعات الناتجة، حيث يتم عرض الأقسام التي تحتوي على أكثر من 5 موظفين فقط.
```

- لا يمكن استخدام `WHERE` بدلاً من `HAVING` في هذه الحالة. السبب:

  - `WHERE`: يُطبق على الصفوف الفردية قبل التجميع للتصفية باستخدام الأعمدة العادية
  - `HAVING`: يُطبق على المجموعات بعد التجميع للتصفية باستخدام دوال التجميع (COUNT, SUM, AVG, etc.)

- مثال توضيحي:

```sql
-- استخدام WHERE (على الصفوف قبل التجميع)
SELECT 
    department_id,
    COUNT(*) as employee_count
FROM employees
WHERE salary > 5000          -- يصفي الموظفين الذين راتبهم > 5000
GROUP BY department_id;

-- استخدام HAVING (على المجموعات بعد التجميع)
SELECT 
    department_id,
    COUNT(*) as employee_count
FROM employees
GROUP BY department_id
HAVING COUNT(*) > 5;         -- يصفي الأقسام التي بها > 5 موظفين
-- لا يمكن استخدام WHERE COUNT(*) > 5 لأن COUNT دالة تجميع تعمل على مجموعة من الصفوف.
```

- ترتيب التنفيذ:

1. `FROM`
2. `WHERE`
3. `GROUP BY`
4. `HAVING`
5. `SELECT`
6. `ORDER BY`

###### JOINS - الربط بين الجداول

```sql
-- إنشاء جداول للربط
CREATE TABLE departments (
    id SERIAL PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    manager_id INTEGER
);

CREATE TABLE projects (
    id SERIAL PRIMARY KEY,
    name VARCHAR(200) NOT NULL,
    budget DECIMAL(12,2),
    department_id INTEGER REFERENCES departments(id)
);
```

**INNER JOIN (المشتركة فقط):**

```sql
SELECT 
    e.first_name,
    e.last_name,
    d.name as department_name
FROM employees e
INNER JOIN departments d ON e.department_id = d.id;
```

*يعرض فقط الموظفين الذين لديهم أقسام*
*لا يعرض الموظفين بدون أقسام*
*لا يعرض الأقسام بدون موظفين*

**LEFT JOIN (جميع السجلات من الجدول الأيسر):**

```sql
SELECT 
    e.first_name,
    e.last_name,
    d.name as department_name
FROM employees e
LEFT JOIN departments d ON e.department_id = d.id;
```

*يعرض جميع الموظفين*
*إذا كان الموظف بدون قسم، يظهر department_name كـ NULL*
*لا يعرض الأقسام بدون موظفين*

**RIGHT JOIN:**

```sql
SELECT 
    e.first_name,
    d.name as department_name
FROM employees e
RIGHT JOIN departments d ON e.department_id = d.id;
```

*يعرض جميع الأقسام*
*إذا كان القسم بدون موظفين، يظهر first_name كـ NULL*
*لا يعرض الموظفين بدون أقسام*

**JOIN متعدد:**

```sql
SELECT 
    e.first_name,
    p.name as project_name,
    d.name as department_name
FROM employees e
INNER JOIN departments d ON e.department_id = d.id
INNER JOIN projects p ON p.department_id = d.id;
```

*يعرض فقط:*
    *الموظفين الذين لديهم أقسام*
    *والأقسام التي لديها مشاريع*
    *ويربط بين الثلاثة (الموظف - القسم - المشروع)*
*لا يعرض أي سجلات بدون ارتباط في أي من الجداول الثلاثة*

###### Subqueries - الاستعلامات الفرعية

**Subquery في WHERE:**

```sql
-- الموظفين الذين راتبهم أكبر من متوسط راتب الموظفين
SELECT first_name, last_name, salary
FROM employees
WHERE salary > (SELECT AVG(salary) FROM employees);
```

**IN مع Subquery:**

```sql
-- الموظفين الذين بقسم التطوير
SELECT first_name, last_name
FROM employees
WHERE department_id IN (
    SELECT id FROM departments WHERE name LIKE '%تطوير%'
);
```

- `department_id` في `employees` مرتبط بـ `id` في `departments` فداخل جدول الموظفين يعرض الموظفين الذي معرف قسمهم موجود داخل معرف جدول الأقسام الذي اسم قسمه خاص بالتطوير

**EXISTS:**

```sql
-- الموظفين الذين لديهم مشروع واحد على الأقل يديرونه
SELECT first_name, last_name
FROM employees e
WHERE EXISTS (
    SELECT 1
    FROM projects p 
    WHERE p.manager_id = e.id
);
```

- الاستعلام الداخلي مرتبط بالصف الخارجي (`correlated subquery`): لكل صف من `employees` يتحقق هل يوجد أي صف في `projects` حيث p.manager_id = e.id.
- إذا وجد صف واحد فقط يَعتبر الشرط `true` وتُرجع السجل.
- استخدام `SELECT 1` شائع لأن القيمة نفسها لا تهم، المهم وجود صف.
- ملاحظة أداء: عادة أسرع من `JOIN` عندما تحتاج فقط للتحقق من الوجود لأن البحث يتوقف عند أول نتيجة.

**Subquery في SELECT:**

```sql
-- يعرض متوسط الشركة ويعرض الفرق لكل موظف
SELECT 
    first_name,
    last_name,
    salary,
    (SELECT AVG(salary) FROM employees) as company_avg_salary,
    salary - (SELECT AVG(salary) FROM employees) as difference -- لو قيمة موجبة يكون فوق المتوسط بهذا المقدار ولو قيمة سالبة يكون تحت المتوسط بهذا المقدار
FROM employees;
```

- *(SELECT AVG(salary) FROM employees):* يحسب متوسط رواتب كل الموظفين (قيمة واحدة).
- العمود `company_avg_salary` سيظهر نفس القيمة لكل صف، وعمود difference = salary - company_avg_salary.

*مثال خاطئ:*

```sql
SELECT
    first_name,
    last_name,
    salary,
    AVG(salary) as company_avg_salary,  -- خطأ
    salary - company_avg_salary as difference  -- خطأ
FROM employees;
```

- سبب الخطأ الأول:
  - عندما تستخدم `AVG(salary)` بدون `GROUP BY`، تتعامل `PostgreSQL` معها كدالة تجميع (`aggregate function`) تطبق على جميع الصفوف، لكنك تحاول أيضاً عرض أعمدة فردية `(first_name, last_name, salary)` بدون تجميع.

- سبب الخطأ الثاني:
  - لا يمكنك استخدام عمود مسمى (`alias`) في نفس `SELECT clause` - حيث يتم تقييم جميع الأعمدة في نفس الوقت

- ملاحظة أداء: بعض قواعد البيانات تحسن وتنفّذ الـ `subquery` مرة واحدة، لكن قد تُنفَّذ لكل صف. أفضل كتابة أكثر كفاءة بهذا الشكل:

  - بديل بحساب المتوسط مرة واحدة عبر الجدول المشتق (`derived table`):

  ```sql
  SELECT e.first_name, e.last_name, e.salary, stats.company_avg_salary,
         e.salary - stats.company_avg_salary AS difference
  FROM employees e
  CROSS JOIN (SELECT AVG(salary) AS company_avg_salary FROM employees) stats;
  ```

  - أو باستخدام وظيفة النافذة (`window function`) أسهل وأكثر فعالية وموصى بها:

  ```sql
  SELECT first_name, last_name, salary,
         AVG(salary) OVER () AS company_avg_salary,
         salary - AVG(salary) OVER () AS difference
  FROM employees;
  ```

  - ولتحسين الاستعلام أكثر:

  ```sql
  SELECT first_name, last_name, salary,
    ROUND(AVG(salary) OVER (), 2) AS company_avg_salary,
    ROUND(salary - AVG(salary) OVER (), 2) AS difference
  FROM employees;
  ```

###### Window Functions - وظائف النافذة

**Ranking Functions - وظائف الترتيب:**

- `Ranking Functions` هي نوع من `Window Functions`تستخدم لتعيين رتب للصفوف ضمن مجموعة معينة. تقدم `PostgreSQL` عدة دوال ترتيب مفيدة:

*دوال الترتيب الرئيسية:*

1. `ROW_NUMBER()`: يعطي رقم صف فريد متسلسل (1, 2, 3, ...) بغض النظر عن القيم المكررة

    ```sql
    SELECT 
        first_name,
        salary,
        department,
        ROW_NUMBER() OVER (ORDER BY salary DESC) as row_num
    FROM employees;
    ```

2. `RANK()`: يعطي ترتيباً مع تكرار وقفزات أو فجوات عند القيم المكررة
   - الراتب: 5000, 5000, 4000, 3000
   - الرتبة: 1, 1, 3, 4 ← لاحظ القفز من 1 إلى 3
   - تفسير القفزات: بعد مجموعة حجم n، الرتبة التالية = (الرتبة الحالية) + n. مثلاً بعد خمس عناصر برتبة 1 تصبح الرتبة التالية 6.

    ```sql
    SELECT 
        first_name,
        salary,
        department,
        RANK() OVER (ORDER BY salary DESC) as rank
    FROM employees;
    ```

3. `DENSE_RANK()`: يعطي ترتيباً مع تكرار بدون قفزات أو فجوات عند القيم المكررة
   - الراتب: 5000, 5000, 4000, 3000
   - الرتبة: 1, 1, 2, 3 ← لا توجد فجوات

    ```sql
    SELECT 
        first_name,
        salary,
        department,
        DENSE_RANK() OVER (ORDER BY salary DESC) as dense_rank
    FROM employees;
    ```

4. `NTILE(n)`: يقسم البيانات إلى `n` مجموعات متساوية قدر الإمكان

    ```sql
    SELECT 
        first_name,
        salary,
        NTILE(4) OVER (ORDER BY salary DESC) as quartile
    FROM employees;
    ```

*مثال عملي:*

````sql
WITH t(val) AS (
  VALUES (100),(100),(100),(100),(100),(90),(90),(90),(80)
)
SELECT val,                                         -- 100   100   100   100   100   90   90   90   80
  ROW_NUMBER() OVER (ORDER BY val DESC) AS rn,      -- 1     2     3     4     5     6     7    8   9
  RANK() OVER (ORDER BY val DESC) AS r,             -- 1     1     1     1     1     6     6    6   9
  DENSE_RANK() OVER (ORDER BY val DESC) AS dr,      -- 1     1     1     1     1     2     2    2   3
  NTILE(4) OVER (ORDER BY val DESC) as n            -- 1     1     1     2     2     3     3    4   4
FROM t;
````

**PARTITION BY - التجميع مع:**

- يمكنك تطبيق الترتيب على مجموعات منفصلة:

```sql
SELECT 
    first_name, last_name, department_id, salary,
    AVG(salary) OVER (PARTITION BY department_id) as dept_avg_salary,  -- متوسط الرواتب لكل قسم
    salary - AVG(salary) OVER (PARTITION BY department_id) as diff_from_avg  -- الفرق بين راتب كل موظف ومتوسط قسمه
FROM employees;

SELECT 
    first_name,
    salary,
    department,
    ROW_NUMBER() OVER (PARTITION BY department ORDER BY salary DESC) as dept_rank,        -- ترتيب لا يسمح بالتكرار لرواتب كل قسم
    RANK() OVER (PARTITION BY department ORDER BY salary DESC) as dept_rank_with_gaps,    -- ترتيب يسمح بالتكرار مع قفزات لرواتب كل قسم
    DENSE_RANK() OVER (PARTITION BY department ORDER BY salary DESC) as dept_dense_rank   -- ترتيب يسمح بالتكرار بدون قفزات لرواتب كل قسم
FROM employees;
```

- أمثلة عملية:

*الموظفون الأعلى راتباً في كل قسم:*

```sql
SELECT *
FROM (
    SELECT 
        first_name,
        department,
        salary,
        ROW_NUMBER() OVER (PARTITION BY department ORDER BY salary DESC) as rank
    FROM employees
) ranked
WHERE rank <= 3;  -- أفضل 3 موظفين في كل قسم
```

*تقسيم الموظفين إلى شرائح:*

```sql
SELECT 
    first_name,
    salary,
    NTILE(4) OVER (ORDER BY salary) as salary_quartile,
    CASE NTILE(4) OVER (ORDER BY salary)
        WHEN 1 THEN 'Low'
        WHEN 2 THEN 'Medium'
        WHEN 3 THEN 'High' 
        WHEN 4 THEN 'Very High'
    END as salary_category
FROM employees;
```

*مقارنة بين دوال الترتيب:*

```sql
SELECT 
    first_name,
    salary,
    ROW_NUMBER() OVER (ORDER BY salary DESC) as row_num,
    RANK() OVER (ORDER BY salary DESC) as rank,
    DENSE_RANK() OVER (ORDER BY salary DESC) as dense_rank
FROM employees
ORDER BY salary DESC;
```

- نصائح مهمة:

  1. *ORDER BY إلزامي* في دوال الترتيب
  2. *PARTITION BY اختياري* - إذا حذفته يطبق على كل البيانات
  3. *الأداء:* استخدام PARTITION BY قد يحسن الأداء مع البيانات الكبيرة
  4. *الفروق بين الدوال:*
     - `ROW_NUMBER()`: أرقام فريدة دائماً
     - `RANK()`: رتب مع فجوات للمتساويين
     - `DENSE_RANK()`: رتب بدون فجوات للمتساويين

- استخدامات شائعة:

  - إنشاء تقارير الترتيب
  - تحديد أعلى/أدنى N عنصر في كل مجموعة
  - تقسيم البيانات إلى شرائح متساوية
  - إزالة البيانات المكررة (باستخدام `ROW_NUMBER()`)

**Cumulative Sum - المجموع التراكمي:**

```sql
SELECT 
    first_name, hire_date, salary,
    SUM(salary) OVER (ORDER BY hire_date) as cumulative_salary
FROM employees;
```

- يحسب مجموع الرواتب تراكمياً حسب تاريخ التوظيف
- كل صف يعرض مجموع الرواتب حتى ذلك التاريخ

##### Phase 3: Performance and Improvement - المرحلة 3: الأداء والتحسين

###### Indexes - الفهـارس

**إدارة الفهارس:**

```sql
-- أنواع الفهارس
CREATE INDEX idx_employees_email ON employees(email);  -- فهرس عادي
CREATE INDEX idx_employees_department_salary ON employees(department_id, salary);  -- فهرس مركب
CREATE UNIQUE INDEX idx_unique_employee_code ON employees(employee_code);  -- فهرس فريد

-- فهارس متخصصة
CREATE INDEX idx_employees_name_lower ON employees(LOWER(first_name));
CREATE INDEX idx_employees_hire_date_year ON employees(EXTRACT(YEAR FROM hire_date));  -- EXTRACT: تستخدم لاستخراج جزء معين من تاريخ أو وقت.

-- فهارس جزئية
CREATE INDEX idx_high_salary_employees ON employees(salary) WHERE salary > 10000;

-- عرض الفهارس
SELECT * FROM pg_indexes WHERE tablename = 'employees'

-- حذف الفهرس
DROP INDEX idx_employees_email;
```

**الفرق بين INDEX و UNIQUE INDEX:**

- الفهرس العادي (`INDEX`)
  - يسرّع عمليات القراءة (`WHERE`, `JOIN`, `ORDER BY`).
  - لا يمنع تكرار القيم — لا يتحقّق من التفرّد.
  - مناسب للأعمدة التي تُستعلم كثيراً بدون حاجة لفرض قواعد.

- الفهرس الفريد (`UNIQUE INDEX`)
  - يؤدي نفس دور الفهرس في التسريع.
  - بالإضافة إلى ذلك يفرض أن تكون القيمة فريدة في العمود (يمنع إدخال قيمة مكررة).
  - يُستخدم لضمان سلامة البيانات (مثلاً `email`, `national_id`).
  - يُنشئ خطأ عند محاولة إدخال قيمة مكررة.

*أمثلة:*

```sql
-- فهرس عادي
CREATE INDEX idx_users_email ON users(email);

-- فهرس فريد
CREATE UNIQUE INDEX ux_users_email ON users(email);

-- أو عن طريق قيد فريد في تعريف الجدول
ALTER TABLE users ADD CONSTRAINT users_email_unique UNIQUE (email);
```

*ملاحظات مهمة:*

- في `PostgreSQL`: `UNIQUE` يسمح بقيم `NULL` متعددة (`NULL` تُعامل كمختلفة). لمنع `NULL` استخدم `NOT NULL` أو فهرس جزئي:

```sql
ALTER TABLE users ALTER COLUMN email SET NOT NULL;
-- أو
CREATE UNIQUE INDEX ux_users_email_notnull ON users(email) WHERE email IS NOT NULL;
```

- الأداء: كلاهما يفيد القراءة؛ الفهرس الفريد يضيف تكلفة تحقق إضافية عند `INSERT`/`UPDATE` (للتأكد من عدم التكرار).
- المفتاح الأساسي (`PRIMARY KEY`) في النهاية هو قيد فريد ويُنشئ فهرس فريد تلقائياً.

**اختبار تحسين استعلام بطيء:**

```sql
-- لديك استعلام بطيء:
SELECT * FROM users
WHERE LOWER(username) = LOWER('ahmed')
AND EXTRACT(YEAR FROM created_at) = 2023;
-- كيف تحسنه؟
```

*نقاط تحسين الاستعلام البطيء مع أمثلة عملية:*

- المشكلة الرئيسية:
  - استخدام دوال على الأعمدة `(LOWER(username))` يمنع استخدام فهارس عادية.
  - `EXTRACT(YEAR FROM created_at)` أيضاً يمنع استخدام فهرس على `created_at` فيجب تحويلها إلى نطاق زمني.

- الحل تعديل الاستعلام أو إضافة فهارس:

1. عدّل الاستعلام لا تستخدم دوال على العمود، واستخدم نطاق للتاريخ:

    ```sql
    SELECT *
    FROM users
    WHERE LOWER(username) = 'ahmed'                -- or username = 'ahmed' if citext used
    AND created_at >= DATE '2023-01-01'
    AND created_at <  DATE '2024-01-01';
    ```

2. أنشئ فهرس تعابيري على `LOWER(username)`:

    ```sql
    CREATE INDEX idx_users_lower_username ON users (LOWER(username));
    CREATE INDEX idx_users_created_at ON users (created_at);
    -- أو فهرس مُركب مفيد للبحث على كلا الشرطين:
    CREATE INDEX idx_users_lower_username_created_at
    ON users (LOWER(username), created_at);
    ```

3. بديل أفضل جعل العمود غير حساس لحالة الأحرف باستخدام `citext`:

    ```sql
    CREATE EXTENSION IF NOT EXISTS citext;
    ALTER TABLE users ALTER COLUMN username TYPE citext;
    CREATE INDEX idx_users_username_ci ON users (username);
    -- الآن استعلامك يمكن أن يكون:
    SELECT * FROM users
    WHERE username = 'ahmed'
    AND created_at >= DATE '2023-01-01' AND created_at < DATE '2024-01-01';
    ```

4. إذا الاستعلام دائمًا على سنة محددة، استخدم فهرس جزئي لزيادة الكفاءة:

    ```sql
    CREATE INDEX idx_users_lower_username_2023
    ON users (LOWER(username))
    WHERE created_at >= DATE '2023-01-01' AND created_at < DATE '2024-01-01';
    ```

5. تحقق بالأدوات: شغل `EXPLAIN ANALYZE` قبل وبعد لتتأكد أن الفهرس يُستخدم ويُحسّن الزمن:

    ```sql
    EXPLAIN ANALYZE
    SELECT ...
    ```

*خلاصة سريعة:*

- تجنّب تطبيق دوال على الأعمدة في `WHERE` إن أردت استعمال الفهارس.
- استبدل `EXTRACT(YEAR, ...)` بشرط نطاقي على `created_at`.
- أنشئ فهارس مناسبة (`expression`, `composite`, أو `citext`) وفحص الأداء بـ `EXPLAIN ANALYZE`.

**الفهرس مثل "فهرس الكتاب" - لا يغير محتوى الكتاب لكنه يسرع عملية البحث.**

*مثال بسيط:*

1. بدون فهرس:

    ```sql
    SELECT * FROM users WHERE email = 'ahmed@example.com';
    -- يبحث في كل سجل في الجدول (Table Scan)
    -- مثل البحث في كتاب صفحة صفحة
    ```

2. مع فهرس:

    ```sql
    CREATE INDEX idx_email ON users(email);
    SELECT * FROM users WHERE email = 'ahmed@example.com';
    -- يستخدم الفهرس للوصول المباشر
    -- مثل استخدام فهرس الكتاب للوصول للصفحة مباشرة
    ```

*نقاط مهمة:*

- ✅ يسرع البحث
- ❌ يأخذ مساحة تخزين إضافية
- ❌ يبطئ عمليات الإدخال/التحديث (لأنه يحدّث الفهرس)
- ⚠️ استخدمه للأعمدة التي تبحث فيها كثيراً

لذلك نستخدمه بحكمة - ليس كل عمود يحتاج فهرساً.

###### Query Performance Analysis - تحليل أداء الاستعلامات

- **`EXPLAIN`**:
  - يظهر خطة التنفيذ المتوقعة فقط
  - لا ينفذ الاستعلام فعلياً
  - أسرع لأنه لا ينفذ الاستعلام

- **`EXPLAIN ANALYZE`**:
  - ينفذ الاستعلام فعلياً ويظهر النتائج الحقيقية
  - يعطي معلومات أدق عن الوقت الفعلي والذاكرة المستخدمة
  - أبطأ لأنه ينفذ الاستعلام

```sql
-- EXPLAIN الأساسي: مجرد خطة تنفيذ بدون تنفيذ
EXPLAIN SELECT * FROM employees WHERE email = 'test@example.com';

-- EXPLAIN ANALYZE: تنفيذ فعلي مع تحليل
EXPLAIN ANALYZE SELECT * FROM employees WHERE email = 'test@example.com';

-- تحليل JOIN
EXPLAIN ANALYZE 
SELECT e.first_name, d.name 
FROM employees e 
INNER JOIN departments d ON e.department_id = d.id;
```

**قراءة النتائج - أهم الأجزاء:**

1. *أنواع الخطط (Plan Types)*

    ```text
    Seq Scan         ← مسح تسلسلي (للجداول الصغيرة)
    Index Scan       ← مسح باستخدام الفهرس (سريع)
    Index Only Scan  ← استخدام الفهرس فقط (أسرع)
    Nested Loop      ← حلقة متداخلة للانضمام
    Hash Join        ← انضمام باستخدام الهاش
    Sort             ← ترتيب البيانات
    ```

2. *Cost - التكلفة*

    ```text
    Cost=0.00..15.30
    │        │
    │        └── التكلفة الإجمالية
    └── التكلفة الأولية (لأول صف)
    ```

3. *Rows - الصفوف*

    ```text
    rows=1000        ← عدد الصفوف المتوقع
    ```

4. *Width - العرض*

    ```text
    width=204        ← متوسط حجم الصف بالبايت
    ```

**أمثلة عملية لفهم أفضل:**

*مسح تسلسلي:*

```sql
EXPLAIN ANALYZE SELECT * FROM employees;

-- النتيجة:
-- Seq Scan on employees  (cost=0.00..25.00 rows=1000 width=136)
--                       (actual time=0.005..0.150 rows=1000 loops=1)
```

*استخدام الفهرس:*

```sql
EXPLAIN ANALYZE SELECT * FROM employees WHERE id = 100;

-- النتيجة:
-- Index Scan using employees_pkey on employees  
-- (cost=0.15..8.17 rows=1 width=136)
-- (actual time=0.010..0.011 rows=1 loops=1)
--   Index Cond: (id = 100)
```

*انضمام بين جدولين:*

```sql
EXPLAIN ANALYZE 
SELECT e.name, d.department_name 
FROM employees e 
JOIN departments d ON e.department_id = d.id;
```

**نصائح احترافية للتحليل:**

1. *ابحث عن هذه المشاكل:*

    - `Seq Scan` على جداول كبيرة (مؤشر مفقود)
    - `Sort` مع `Disk` (الترتيب يستخدم القرص بدلاً الذاكرة)
    - `rows` الفعلي مختلف كثيراً عن المتوقع (إحصائيات قديمة)

2. *مؤشرات الأداء الجيد:*

   - استخدام `Index Scan` بدلاً من `Seq Scan`
   - `Heap Fetches` قليلة في `Index Only Scan`
   - `Buffers: shared hit` عالي (البيانات في الذاكرة)

3. *استخدم هذه الإعدادات لمعلومات أكثر:*

    ```sql
    EXPLAIN (ANALYZE, BUFFERS, FORMAT JSON) 
    SELECT * FROM table;
    ```

**مثال تحليل متقدم:**

*إنشاء الجداول:*

```sql
-- جدول العملاء
CREATE TABLE customers (
    id SERIAL PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    email VARCHAR(100),
    phone VARCHAR(20),
    address TEXT,
    created_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-- جدول الطلبات
CREATE TABLE orders (
    id SERIAL PRIMARY KEY,
    customer_id INTEGER REFERENCES customers(id),
    order_date DATE NOT NULL,
    status VARCHAR(20) DEFAULT 'pending',
    total_amount DECIMAL(10,2),
    shipping_address TEXT,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-- جدول عناصر الطلبات
CREATE TABLE order_items (
    id SERIAL PRIMARY KEY,
    order_id INTEGER REFERENCES orders(id),
    product_name VARCHAR(200) NOT NULL,
    quantity INTEGER NOT NULL,
    unit_price DECIMAL(10,2) NOT NULL,
    amount DECIMAL(10,2) NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-- إنشاء الفهارس لتحسين الأداء
CREATE INDEX idx_orders_customer_id ON orders(customer_id);
CREATE INDEX idx_orders_order_date ON orders(order_date);
CREATE INDEX idx_order_items_order_id ON order_items(order_id);
CREATE INDEX idx_customers_name ON customers(name);
```

*إدخال البيانات:*

```sql
-- إدخال عملاء
INSERT INTO customers (name, email, phone, address) VALUES
('أحمد محمد', 'ahmed@email.com', '0123456789', 'القاهرة - مصر الجديدة'),
('فاطمة علي', 'fatima@email.com', '0123456790', 'الإسكندرية - سموحة'),
('محمد السيد', 'mohamed@email.com', '0123456791', 'الجيزة - الدقي'),
('سارة خالد', 'sara@email.com', '0123456792', 'الرياض - العليا'),
('ياسمين أحمد', 'yasmin@email.com', '0123456793', 'جدة - الصفا'),
('خالد عبدالله', 'khaled@email.com', '0123456794', 'الدمام - الظهران'),
('نورا سعد', 'nora@email.com', '0123456795', 'أبوظبي - المركز'),
('عمر حسن', 'omar@email.com', '0123456796', 'دبي - ديرة'),
('لينا محمود', 'lena@email.com', '0123456797', 'الشارقة - النهدة'),
('ياسر فاروق', 'yasser@email.com', '0123456798', 'العين - القطارة')
RETURNING id;  -- هذا يعرض الـ IDs التي تم إدخالها

-- التحقق من IDs الحقيقية للعملاء
SELECT id, name FROM customers ORDER BY id;

-- إدخال 1000 طلب (بين 2023 و 2024)
INSERT INTO orders (customer_id, order_date, status, total_amount, shipping_address) 

-- SELECT (orders records) FROM generate_series(1, 1000)
SELECT 
    -- customer_id
    (SELECT id FROM customers ORDER BY random() LIMIT 1)  -- أي معرف عشوائي من جدول العملاء

    -- order_date
    DATE '2023-01-01' + (random() * 730)::int,
    -- DATE '2023-01-01' ← تاريخ البداية
    -- random() * 730 ← رقم بين 0 و 730 (سنتين = 730 يوم)
    -- النتيجة: تاريخ عشوائي بين 2023-01-01 و 2024-12-30

    -- status
    (CASE (random() * 3)::int 
        WHEN 0 THEN 'pending' 
        WHEN 1 THEN 'shipped' 
        ELSE 'delivered' 
     END),
    -- (random() * 3)::int ← رقم 0 أو 1 أو 2
    -- WHEN 0 THEN 'pending' ← إذا 0 يكون pending
    -- WHEN 1 THEN 'shipped' ← إذا 1 يكون shipped
    -- ELSE 'delivered' ← إذا 2 يكون delivered

    -- total_amount
    (random() * 1000 + 50)::decimal(10,2),
    -- random() * 1000 ← بين 0 و 1000
    -- + 50 ← بين 50 و 1050
    -- النتيجة: مبلغ عشوائي بين 50.00 و 1050.00

    -- shipping_address
    'عنوان الشحن'

-- 1000 سجل
FROM generate_series(1, 1000);
-- ينشئ 1000 صف (من 1 إلى 1000)
-- مثل عمل loop لـ 1000 مرة

-- التحقق من الطلبات
SELECT COUNT(*) as total_orders FROM orders;
SELECT customer_id, COUNT(*) FROM orders GROUP BY customer_id;

-- إدخال 4 عناصر طلبات
INSERT INTO order_items (order_id, product_name, quantity, unit_price, amount)

-- CTE
WITH items_data AS (
    -- SELECT (order_items records) FROM orders CROSS JOIN generate_series(1, (floor(random() * 3) + 1)::int);
    SELECT 

        -- order_id
        o.id as order_id,
        -- يؤخذ من جدول الطلبات

        -- product_name
        ('منتج ' || (floor(random() * 20) + 1)::int) as product_name,
        -- (random() * 20 + 1)::int ← رقم بين 1 و 21
        -- 'منتج ' || ... ← دمج النص مع الرقم
        -- النتيجة: "منتج 1" إلى "منتج 21"

        -- quantity
        (floor(random() * 5) + 1)::int as quantity,  -- كمية بين 1 و 6

        -- unit_price
        (random() * 200 + 10)::decimal(10,2) as unit_price,  -- سعر الوحدة بين 10.00 و 210.00

        -- amount
        -- حساب المبلغ = الكمية × سعر الوحدة
        -- quantity * unit_price
        ((random() * 5 + 1)::int * (random() * 200 + 10))::decimal(10,2) as item_amount

    -- أخذ جميع الطلبات (1000 طلب)
    FROM orders o

    CROSS JOIN generate_series(1, (floor(random() * 3) + 1)::int)
    -- (random() * 3 + 1)::int ← رقم بين 1 و 4
    -- generate_series(1, X) ← ينشئ X أسطر لكل طلب
    -- النتيجة: كل طلب سيكون له بين 1 و 4 عناصر
)
SELECT 
    -- الأسماء في CTE
    order_id,
    product_name,
    quantity,
    unit_price,
    (quantity * unit_price) as amount
FROM items_data;

-- التحقق من عدد عناصر الطلبات المدرجة
SELECT COUNT(*) as total_order_items FROM order_items;

-- التحقق من توزيع العناصر لكل طلب
SELECT order_id, COUNT(*) as items_count 
FROM order_items 
GROUP BY order_id 
ORDER BY items_count DESC 
LIMIT 10;

-- تحديث بعض الطلبات لتكون في 2024
UPDATE orders 
SET order_date = DATE '2024-01-01' + (floor(random() * 200))::int
-- DATE '2024-01-01' ← تاريخ البداية
-- (random() * 200)::int ← بين 0 و 200 يوم
-- النتيجة: تاريخ بين 2024-01-01 و 2024-07-19

WHERE id IN (SELECT id FROM orders ORDER BY random() LIMIT 300);
-- ORDER BY random() ← يخلط الطلبات عشوائياً
-- LIMIT 300 ← يأخذ 300 طلب عشوائي
-- النتيجة: تحديث 300 طلب عشوائي

-- تحديث المبلغ الإجمالي للطلبات
UPDATE orders o
SET total_amount = (
    SELECT SUM(amount) 
    FROM order_items oi 
    WHERE oi.order_id = o.id
);

-- بعد تنفيذ هذه الاستعلامات:
-- العملاء: 10 عملاء
-- الطلبات: 1000 طلب
-- 700 طلب في 2023
-- 300 طلب في 2024
-- عناصر الطلبات: ≈ 2500 عنصر (بين 1-4 عنصر لكل طلب)
```

*تشغيل الاستعلام مع التحليل:*

```sql
-- الآن يمكننا تشغيل EXPLAIN ANALYZE
EXPLAIN (ANALYZE, BUFFERS, VERBOSE) 
SELECT 
    o.order_date, 
    c.name, 
    SUM(oi.amount) as total_amount
FROM orders o
JOIN customers c ON o.customer_id = c.id
JOIN order_items oi ON o.id = oi.order_id
WHERE o.order_date >= '2024-01-01'
GROUP BY o.order_date, c.name
ORDER BY SUM(oi.amount) DESC
LIMIT 10;
```

*استعلامات مساعدة للتحليل:*

```sql
-- عرض إحصائيات البيانات
SELECT 
    (SELECT COUNT(*) FROM customers) as customers_count,
    (SELECT COUNT(*) FROM orders) as orders_count,
    (SELECT COUNT(*) FROM order_items) as order_items_count,
    (SELECT COUNT(*) FROM orders WHERE order_date >= '2024-01-01') as orders_2024;

-- تحليل الفهارس
SELECT 
    tablename, 
    indexname, 
    indexdef 
FROM pg_indexes 
WHERE tablename IN ('customers', 'orders', 'order_items');

-- تحليل توزيع البيانات
SELECT 
    order_date,
    COUNT(*) as order_count
FROM orders 
GROUP BY order_date 
ORDER BY order_date DESC 
LIMIT 10;
```

*استعلامات إضافية للتدريب:*

```sql
-- 1. تحليل بدون BUFFERS
EXPLAIN ANALYZE 
SELECT o.order_date, c.name, SUM(oi.amount)
FROM orders o
JOIN customers c ON o.customer_id = c.id
JOIN order_items oi ON o.id = oi.order_id
WHERE o.order_date >= '2024-01-01'
GROUP BY o.order_date, c.name
ORDER BY SUM(oi.amount) DESC
LIMIT 10;

-- 2. تحليل مع FORMAT مختلف
EXPLAIN (ANALYZE, FORMAT JSON) 
SELECT o.order_date, c.name, SUM(oi.amount)
FROM orders o
JOIN customers c ON o.customer_id = c.id
JOIN order_items oi ON o.id = oi.order_id
WHERE o.order_date >= '2024-01-01'
GROUP BY o.order_date, c.name
ORDER BY SUM(oi.amount) DESC
LIMIT 10;
```

**لماذا نستخدم EXPLAIN ANALYZE:**

*تخيل أنك تريد السفر من الرياض إلى جدة. هناك عدة طرق:*

1. الطريق السريع (أسرع)
2. الطريق العادي (أبطأ)
3. طريق غير معبد (أبطأ كثيراً)

*`EXPLAIN ANALYZE` هو مثل خرائط جوجل يخبرك:*

- أي طريق اخترت قاعدة البيانات؟
- كم وقت استغرقت الرحلة؟
- كم بنزين استهلكت؟

**لنحلل النتيجة معاً خطوة بخطوة:**

*الجزء الأول: أين قضت قاعدة البيانات معظم وقتها:*

- ابحث عن السطر الذي فيه أكبر رقم في `actual time`:

```text
->  Seq Scan on orders o  (actual time=0.008..15.320 rows=285 loops=1)
```

هنا قاعدة البيانات قضت 15.3 ميلي ثانية في قراءة جدول الطلبات.

*الجزء الثاني: هل استخدمت الفهرس أم لا:*

- `Seq Scan` = قراءة كل الجدول (سيء للجداول الكبيرة)
- `Index Scan` = استخدام الفهرس (جيد)

*الجزء الثالث: (كم صف قرأت vs كم صف وجدت فعلاً):*

```text
rows=500  ← توقعت 500 صف
actual rows=285  ← لكن وجدت 285 فقط
```

إذا الفرق كبير، معناه أن إحصائيات قاعدة البيانات قديمة.

**ماذا أفعل بهذه المعلومات:**

*إذا رأيت `Seq Scan` على جدول كبير:*

```sql
-- أضف فهرساً
CREATE INDEX idx_orders_date ON orders(order_date);
```

*إذا رأيت `Sort` مكلف:*

```sql
-- حاول استخدام ORDER BY مختلف
```

*إذا رأيت تقديرات خاطئة:*

```sql
-- حدّث الإحصائيات
ANALYZE orders;
```

**النتيجة النهائية التي تريدها:**

*بعد تحليل `EXPLAIN ANALYZE` ستكتشف أن:*

- المشكلة كانت في عدم وجود فهرس على `order_date`
- الحل إضافة الفهرس
- التحسن الاستعلام أصبح أسرع 10 مرات

**مثال عملي مبسط:**

```sql
-- قبل التحسين: 100 ميلي ثانية
EXPLAIN ANALYZE SELECT * FROM orders WHERE order_date >= '2024-01-01';

-- نلاحظ: Seq Scan - بطيء

-- نضيف الفهرس
CREATE INDEX idx_orders_date ON orders(order_date);

-- بعد التحسين: 10 ميلي ثانية  
EXPLAIN ANALYZE SELECT * FROM orders WHERE order_date >= '2024-01-01';

-- نلاحظ: Index Scan - سريع
```

**الخلاصة:**

*`EXPLAIN ANALYZE` ليس هدف في نفسه، بل وسيلة لاكتشاف المشاكل وإصلاحها لجعل استعلاماتك أسرع وأكثر كفاءة.*

**تجربة تشغيل الاستعلام من جديد لتحليله:**

*التحليل المبسط للنتيجة:*

1. الأداء العام ممتاز

    ```text
    Execution Time: 1.322 ms
    ```

    الاستعلام استغرق 1.3 ميلي ثانية فقط - هذا سريع جداً!

2. أين قضى معظم الوقت؟

   - `0.546 ms`: في تجميع الطلبات مع عناصرها
   - `0.111 ms`: في قراءة عناصر الطلبات  
   - `0.079 ms`: في قراءة الطلبات

3. المشاكل المحتملة:

    ```text
    Seq Scan on public.orders
    Seq Scan on public.order_items  
    Seq Scan on public.customers
    ```

    كل الجداول تُقرأ بالمسح التسلسلي - لكن هذا مقبول لأن البيانات قليلة.

*الإيجابيات:*

- ⚡ سرعة ممتازة (1.3 ميلي ثانية)
- 💾 استخدام ذاكرة قليل (209 كيلوبايت فقط)
- 🔄 لا مشاكل أداء تذكر

*السلبيات الطفيفة:*

- يمكن تحسينه أكثر ببعض الفهارس

*كيف يمكن تحسينه أكثر:*

- إضافة فهارس ستحسنه قليلاً:

```sql
CREATE INDEX idx_orders_date_customer ON orders(order_date, customer_id);
CREATE INDEX idx_order_items_order_id ON order_items(order_id);
```

لكن الفرق سيكون طفيفاً لأن الاستعلام سريع أصلاً

*متى تقلق من نتائج EXPLAIN ANALYZE:*

- قلق إذا رأيت:
  - `Execution Time` أكثر من 100 ميلي ثانية
  - `Seq Scan` على جداول بها آلاف الصفوف
  - `Sort` مع `Disk` بدل `Memory`
  - `Rows Removed by Filter` أعداد كبيرة

**خطوات التحليل الاحترافي:**

1. *حدد أبطأ جزء في خطة التنفيذ*
2. *ابحث عن عمليات المسح التسلسلي على البيانات الكبيرة*
3. *تحقق من دقة تقديرات الصفوف*
4. *ابحث عن عمليات الترتيب والانضمام المكلفة*
5. *اقترح الحلول (إضافة فهارس، إعادة كتابة الاستعلام، إلخ)*

**تمارين عملية للتدريب:**

1. قارن بين `EXPLAIN` و `EXPLAIN ANALYZE` على استعلام بسيط
2. جرب إضافة `WHERE` مختلفة وشاهد كيف تتغير خطة التنفيذ
3. أنشئ فهرساً وشاهد الفرق في الأداء
4. حلل استعلامات معقدة تحتوي على `JOIN` و `GROUP BY`

###### Advanced Optimization - التحسين المتقدم

**نصائح التحسين:**

```sql
-- 1. تجنب SELECT *
SELECT id, first_name, last_name FROM employees; -- أفضل

-- 2. استخدام الفهارس المناسبة
CREATE INDEX idx_composite ON table(col1, col2, col3);

-- 3. تجنب الدوال على الأعمدة المفهرسة
-- سيء: لا يستخدم الفهرس
SELECT * FROM employees WHERE LOWER(email) = 'test@example.com';

-- جيد: يستخدم الفهرس
SELECT * FROM employees WHERE email = 'test@example.com';

-- 4. استخدام LIMIT للبيانات الكبيرة
SELECT * FROM large_table ORDER BY id LIMIT 1000;
```

###### Transactions - المعاملات

*التعريف:*

- المعاملة مجموعة من عبارات `SQL` تنفَّذ كوحدة واحدة؛ إما تُلتزم كلها (`COMMIT`) أو تُتراجع كلها (`ROLLBACK`).

*الهدف:*

- تضمن أن جميع العمليات (الاستعلامات) تُنفذ بنجاح أو لا شيء يُنفذ على الإطلاق.

- ضمان الاتساق والموثوقية عبر خصائص `ACID`:
  - `Atomicity` (الذرّية): إما كل التغييرات تُطبّق أو لا شيء.
  - `Consistency` (الاتساق): تحافظ القاعدة على القيود والقواعد بعد المعاملة.
  - `Isolation` (العزل): كل معاملة ترى حالة قاعدة مناسبة وفق مستوى العزل.
  - `Durability` (الدوام): بعد `COMMIT`، التغييرات محفوظة حتى عند فشل النظام.

*السلوك:*

- إذا كان هناك استعلام واحد خاطئ في مجموعة من الاستعلامات، يتم إلغاء جميع التغييرات (`ROLLBACK`) — وهذا يضمن عدم وجود حالة غير متسقة في قاعدة البيانات.

*مثال:*

- إذا كنت تقوم بتحويل أموال بين حسابين، إذا فشل أحد التحديثات (مثل خصم من حساب وعدم إضافة إلى الآخر)، فإن المعاملة ستتراجع بالكامل.

*الشبه:*

- فكرة `Transactions` مشابهة لـ `try`/`except` في بايثون فتكون المعاملة (`TRANSACTION`) مثل `try`

*مثال نموذجي:*

```sql
-- المعاملات الأساسية
BEGIN;  -- بدء المعاملة

UPDATE accounts SET balance = balance - 1000 WHERE id = 1;
UPDATE accounts SET balance = balance + 1000 WHERE id = 2;

-- تنفيذ كل العمليات في حالة نجاح كل العمليات
COMMIT;

-- إلغاء تنفيذ كل العمليات في حالة حدوث خطأ لأي عملية
ROLLBACK;

-- مثال عملي
BEGIN;
INSERT INTO orders (order_date) VALUES (CURRENT_DATE);
INSERT INTO order_items (order_id, product_id, quantity) 
VALUES (currval('orders_id_seq'), 1, 2);
COMMIT;

-- مستويات العزل
SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
```

*ماذا سيحدث بدون معاملات (أو بدون استخدامها بشكل صحيح)؟:*

- تحديثات جزئية: جزء من العملية ينفّذ والجزء الآخر يفشل فتظهر بيانات غير متسقة (مثلاً تحويل أموال يحدث طرف واحد فقط).
- مشاكل تزامن (`Concurrency`): تعارضات، `lost updates`، أو قراءات غير متوقعة بين المعاملات المتزامنة.
- صعوبة الاسترداد: لا توجد وسيلة سهلة للتراجع عند خطأ.
- قد تُخالف قيود التكامل أثناء عملية متعددة الخطوات.

**SAVEPOINT:**

*التعريف:*

- يسمح بعمل نقطة استرجاع داخل المعاملة يمكن الرجوع إليها بدون إلغاء كل التغييرات أي يمكنك التراجع جزئياً بدل `ROLLBACK` كامل.  

*الهدف:*

- يسمح لك بإنشاء نقطة استرجاع داخل المعاملة، مما يتيح لك التراجع إلى تلك النقطة دون إلغاء المعاملة بالكامل.

*السلوك:*

- يمكنك تنفيذ عدة استعلامات، وإذا حدث خطأ في أحدها، يمكنك التراجع فقط إلى `SAVEPOINT`، مما يعني أن الاستعلامات التي تمت قبل `SAVEPOINT` ستظل سارية.

*مثال:*

- إذا كنت تضيف طلبًا جديدًا مع عناصر متعددة، يمكنك استخدام `SAVEPOINT` قبل إدخال العناصر. إذا فشل إدخال عنصر واحد، يمكنك التراجع فقط إلى `SAVEPOINT`، مما يسمح لك بإدخال الطلب دون العناصر المفقودة، بدلاً من إلغاء الطلب بالكامل.

*الفائدة من `SAVEPOINT`:*

- المرونة:
  - يسمح لك بالتعامل مع الأخطاء بشكل أكثر دقة. بدلاً من إلغاء كل شيء، يمكنك معالجة الأخطاء بشكل جزئي.

- تحسين الأداء:
  - في بعض الحالات، قد ترغب في تنفيذ بعض العمليات حتى لو فشلت أخرى، مما يسمح لك بالاستمرار في العمل مع البيانات المتاحة.

- تجنب التعارضات:
  - في العمليات المعقدة، قد يكون لديك استعلامات متعددة، وتريد التأكد من أن بعضها يمكن أن يستمر حتى لو فشل البعض الآخر.

*أمثلة قصيرة:*

1. استخدام `SAVEPOINT` في `SQL` عادي

    ```sql
    BEGIN;
    INSERT INTO orders (customer_id) VALUES (1);  -- إنشاء طلب
    SAVEPOINT sp_item;

    -- محاولة إدخال عنصر قد تفشل
    INSERT INTO order_items (order_id, product_id, quantity)
    VALUES (currval('orders_id_seq'), 999, 1);

    -- لو اكتشفت خطأ أو فشل: عد إلى النقطة دون إلغاء بقية المعاملة
    ROLLBACK TO SAVEPOINT sp_item;

    -- أو لو نجح كل شيء تخلص من الـ savepoint
    RELEASE SAVEPOINT sp_item;

    COMMIT;
    ```

2. نمط `PL`/`pgSQL` (الطريقة المفضلة لمعالجة الأخطاء داخل الخادم — يمثل `BEGIN..EXCEPTION subtransaction` تلقائياً)

    ```sql
    DO $$
    BEGIN
    INSERT INTO orders (customer_id) VALUES (1);

    BEGIN
        -- هذه البلوك تعمل كـ subtransaction (savepoint)
        INSERT INTO order_items (order_id, product_id, quantity)
        VALUES (currval('orders_id_seq'), 999, 1);
    EXCEPTION WHEN foreign_key_violation THEN
        -- تعامل مع الخطأ واستمر — لم يتم إلغاء المعاملة الكاملة
        RAISE NOTICE 'منتج غير موجود، تم تخطي إدخال العنصر';
    END;

    -- تابع عمليات أخرى
    INSERT INTO shipments (order_id, ship_date) VALUES (currval('orders_id_seq'), CURRENT_DATE);

    END;
    $$ LANGUAGE plpgsql;
    ```

*نقاط عملية قصيرة:*

- `PostgreSQL` في الوضع الافتراضى يعمل بـ `autocommit`: كل عبارة تُعد معاملة منفصلة ما لم تبدأ `BEGIN`.
- استخدم `SAVEPOINT` لتجزئة المعاملة وإمكانية التراجع الجزئي.
- اختبر الأداء ومستوى العزل حسب الحاجة (`READ COMMITTED`، `REPEATABLE READ`، `SERIALIZABLE`).

*ملاحظات مهمة مختصرة:*

- `ROLLBACK TO SAVEPOINT`: يعيد الحالة للنقطة المحددة دون إنهاء المعاملة.
- `RELEASE SAVEPOINT`: يحذف النقطة (اختياري).
- في حالات أخطاء غير معالجة على مستوى الجلسة قد تحتاج صراحةً لاستخدام `ROLLBACK`؛ `SAVEPOINT` أو `EXCEPTION` داخل `PL`/`pgSQL` لأنه يسمح بالاستمرار بعد الأخطاء الصغيرة.

**Transaction Isolation - مستويات العزل:**

- *في `PostgreSQL` وفي أنظمة قواعد البيانات عمومًا، عند تنفيذ أكثر من معاملة (`Transaction`) في نفس الوقت، قد تتداخل هذه العمليات مع بعضها — مثلاً تعديل نفس الجدول أو قراءة بيانات يجري تعديلها الآن، فلمنع هذه المشكلات، وُجدت ما تُعرف بمستويات العزل (`Transaction Isolation Levels`)، أي كم درجة الانفصال بين المعاملات.*

- الفكرة باختصار كل مستوى من مستويات العزل يوازن بين:
  1. `Performance`: الأداء
  2. `Consistency`: دقة البيانات

- كلما زاد العزل زادت الدقة ولكن قلّ الأداء
- وكلما قل العزل زاد الأداء ولكن زادت احتمالية تضارب البيانات

*أنواع المشكلات التي نحاول تجنبها:*

| نوع المشكلة             | الوصف                                                           |
| ----------------------- | --------------------------------------------------------------- |
| `Dirty Read`            | معاملة تقرأ بيانات غير مُثبتة من معاملة أخرى (قد تتراجع لاحقًا) |
| `Non-Repeatable Read`   | نفس الاستعلام يعطي نتائج مختلفة داخل نفس المعاملة               |
| `Phantom Read`          | تظهر أو تختفي صفوف جديدة بين قراءتين متتاليتين في نفس المعاملة  |

- مثال موجز لـ `non-repeatable read` (مسموح في مستوى `READ COMMITTED`):

```sql
BEGIN;
SELECT balance FROM accounts WHERE id=1;  -- يرى 100
UPDATE accounts SET balance=200 WHERE id=1;
COMMIT;

SELECT balance FROM accounts WHERE id=1;  -- في READ COMMITTED سيرى 200 (تغير بين العبارتين)
```

*نقاط سريعة ومباشرة:*

- ماذا يعني عملياً؟
  - كل عبارة `SQL` داخل المعاملة ترى فقط البيانات التي تم الالتزام بها (`committed`) قبل بدء تلك العبارة (`statement`), وليس قبل بدء المعاملة بأكملها.
  - لا ترى بيانات غير مُلتزمة أي لا توجد مشكلة `dirty reads`.
  - ترى تغييرات التزمت خلال المعاملة من قبل معاملات أخرى بين العبارات لذلك قد تحصل على مشاكل `non-repeatable reads` و `phantoms`.

- أين تضعه؟
  - يجب تنفيذه في بداية المعاملة بعد `BEGIN` إن أردت تغييره فقط لتلك المعاملة:

    ```sql
    BEGIN;
    SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
    -- عبارات SQL هنا
    COMMIT;
    ```

  - لتغييره على مستوى الجلسة:

    ```sql
    SET SESSION CHARACTERISTICS AS TRANSACTION ISOLATION LEVEL READ COMMITTED;
    ```

*مستويات العزل الأربعة في `PostgreSQL`*

- `PostgreSQL` يتبع معيار `SQL Standard` (`ANSI`) ويُوفر 4 مستويات:

1. `READ UNCOMMITTED`: أضعف مستوى ولا يمنع شيئًا لكن `PostgreSQL` يعامله مثل `READ COMMITTED` فعليًا
2. `READ COMMITTED`: المستوى الافتراضي في `PostgreSQL` يمنع `"Dirty Reads"` فقط
3. `REPEATABLE READ`: يمنع `"Dirty"` و `"Non-Repeatable Reads"` وهو ممتاز للتقارير والتحليلات
4. `SERIALIZABLE`: يمنع كل أنواع المشكلات (أعلى أمان) لكنه أبطأ ويستهلك موارد أكثر

*شرح تفصيلي لكل مستوى:*

1. `READ UNCOMMITTED`:

    > الأدنى في العزل لكن في `PostgreSQL` لا يختلف عن `READ COMMITTED` فعليًا

    - الخصائص:
      - يسمح بقراءة بيانات غير مُثبتة أي يمنع `"Dirty Reads"` في `PostgreSQL` نظريًا لا فعليًا
      - نادرًا ما يُستخدم
      - في `PostgreSQL`: يُعامل مثل `READ COMMITTED`

2. `READ COMMITTED` (الافتراضي):

    - مستوى العزل `READ COMMITTED` هو المستوى الافتراضي في `PostgreSQL`، وهو يضمن:

    1. *لا قراءة غير مؤكدة (No Dirty Reads)*
        - لا يمكن رؤية البيانات التي لم يتم تأكيدها (`commit`) من المعاملات الأخرى

    2. *يمكن حدوث قراءة غير متكررة (Nonrepeatable Reads)*
        - يمكن أن تتغير البيانات بين قراءتين في نفس المعاملة إذا تم تأكيد تغييرات من معاملة أخرى

    > كل استعلام يرى فقط البيانات التي تم تثبيتها (`Committed`) قبل بدء هذا الاستعلام.

    - الخصائص:
      - يمنع `Dirty Reads`
      - لكن يمكن أن يحدث `Non-Repeatable Reads` أي إذا عدّل أحدهم الصف بعد قراءته

    - مثال:

      - معاملة A تقرأ صفًا.
      - معاملة B تُحدث نفس الصف وتعمل `COMMIT`.
      - معاملة A تقرأ الصف مرة أخرى وترى التعديل الجديد.

    - مثال توضيحي:

    ```sql
    -- المعاملة الأولى (الجلسة 1)
    BEGIN;
    SET TRANSACTION ISOLATION LEVEL READ COMMITTED;

    SELECT balance FROM accounts WHERE id = 1;  -- نفترض الرصيد 1000
    -- معاملة أخرى تغير الرصيد وتؤكد التغيير
    SELECT balance FROM accounts WHERE id = 1;  -- قد نرى الرصيد الجديد
    COMMIT;

    -- المعاملة الثانية (الجلسة 2)
    BEGIN;
    UPDATE accounts SET balance = 2000 WHERE id = 1;
    COMMIT;
    ```

    - مفيد للأداء العالي والمعاملات اليومية مثل `CRUD`.

    - باختصار: هذا يضبط مستوى عزل المعاملات (`transaction isolation`) للمعاملة الحالية إلى المستوى الافتراضي `READ COMMITTED`

3. `REPEATABLE READ`:

    > كل استعلام داخل نفس المعاملة يرى صورة ثابتة للبيانات *(نفس `snapshot`)* كما كانت عند بداية المعاملة حتى وإن حدث أي تغيير.

    - الخصائص:

    - يمنع `Dirty Reads` و `Non-Repeatable Reads`
    - لكن قد تحدث `Phantom Reads` صفوف جديدة تظهر بين قراءتين

    - مثال:

    - معاملة A تنفذ `SELECT * FROM users WHERE age > 20`
    - معاملة B تُضيف مستخدمًا جديدًا `age=25` وتعمل `COMMIT`
    - لو أعادت A تنفيذ نفس الاستعلام لن ترى الصف الجديد

    - يستخدم في العمليات التحليلية حيث نريد ثبات الصورة.

4. `SERIALIZABLE`

    > أقوى مستوى عزل: يجعل كل المعاملات كأنها نُفذت واحدة بعد الأخرى (تسلسليًا).

    - الخصائص:

    - يمنع كل أنواع المشكلات (`Dirty` / `Non-Repeatable` / `Phantom Reads`)
    - `PostgreSQL` يُنفذ ذلك عبر `Serializable Snapshot Isolation` (`SSI`) أي يُراقب التعارضات ديناميكيًا وليس عبر القفل الكامل فقط.

    - العيب:

    - أبطأ، وقد ينتج خطأ `serialization_failure` إن حصل تعارض.

    - يستخدم في العمليات الحرجة ماليًا أو الحساسة جدًا.

*تغيير مستوى العزل في `PostgreSQL`:*

- يمكنك تحديد مستوى العزل بـ 3 طرق:

1. داخل جلسة واحدة:

    ```sql
    SET TRANSACTION ISOLATION LEVEL REPEATABLE READ;
    ```

2. عند بدء المعاملة:

    ```sql
    BEGIN TRANSACTION ISOLATION LEVEL SERIALIZABLE;
    -- أو:
    START TRANSACTION ISOLATION LEVEL SERIALIZABLE;
    ```

3. بشكل افتراضي لكل جلسة:

    ```sql
    SET DEFAULT_TRANSACTION_ISOLATION TO 'read committed';
    ```

- ملخص سريع بالجدول:

| المستوى          | Dirty Read | Non-Repeatable Read | Phantom Read | الأداء      |
| ---------------- | ---------- | ------------------- | ------------ | ----------- |
| READ UNCOMMITTED | ✅ ممكن     | ✅ ممكن              | ✅ ممكن       | ⚡ سريع جدًا |
| READ COMMITTED   | ❌ لا       | ✅ ممكن              | ✅ ممكن       | ⚡ سريع      |
| REPEATABLE READ  | ❌ لا       | ❌ لا                | ✅ ممكن       | ⚖️ متوسط    |
| SERIALIZABLE     | ❌ لا       | ❌ لا                | ❌ لا         | 🐢 أبطأ     |

###### Views

```sql
-- إنشاء View
CREATE VIEW employee_details AS
SELECT 
    e.id,
    e.first_name,
    e.last_name,
    e.salary,
    d.name as department_name,
    p.name as project_name
FROM employees e
LEFT JOIN departments d ON e.department_id = d.id
LEFT JOIN projects p ON p.department_id = d.id;

-- استخدام View
SELECT * FROM employee_details WHERE department_name = 'تطوير';

-- Updatable View
CREATE VIEW active_employees AS
SELECT id, first_name, last_name, email
FROM employees
WHERE is_active = true;

-- Materialized View (لتحسين الأداء)
CREATE MATERIALIZED VIEW department_stats AS
SELECT 
    d.name,
    COUNT(e.id) as employee_count,
    AVG(e.salary) as avg_salary
FROM departments d
LEFT JOIN employees e ON d.id = e.department_id
GROUP BY d.id, d.name;

REFRESH MATERIALIZED VIEW department_stats;
-- يعيد حساب الاستعلام وتحديث البيانات المخزّنة
-- بعد إضافة/تعديل موظفين جدد، البيانات المخزّنة تصبح قديمة
-- هذا السطر يحدثها ليعكس الحالة الحالية للجداول الأساسية
```

**Regular View \ Materialized View:**

- *Regular View - View العادية*: استعلام مخزّن، يُنفّذ في كل مرة تستدعيه يحسب النتيجة فوراً من الجداول الأساسية.
- *Materialized View*: استعلام مخزّن والنتائج مخزّنة فعلياً على القرص، مثل جدول مؤقت.

*المقارنة السريعة:*

| المميز | View عادية | Materialized View |
|--------|-----------|-------------------|
| التخزين | لا (استعلام فقط) | نعم (نتائج مخزّنة) |
| السرعة | بطيء (يحسب كل مرة) | سريع جداً (بيانات جاهزة) |
| الحجم | لا يأخذ مساحة | يأخذ مساحة على القرص |
| البيانات | دائماً محدثة | قد تكون قديمة (محتاج تحديث) |
| الفهارس | لا يمكن | يمكن إنشاء فهارس عليها |

*متى تستخدم كل واحدة؟:*

- *Regular View*: عندما تريد دائماً البيانات الحالية، أو الاستعلام بسيط وسريع
- *Materialized View*: عندما يكون الاستعلام معقد وبطيء، وتقبل ببيانات قليلة التأخر

*أمثلة عملية:*

```sql
-- 1) إنشاء view عادية
CREATE VIEW employee_summary AS
SELECT 
    department_id,
    COUNT(*) as emp_count,
    AVG(salary) as avg_salary
FROM employees
GROUP BY department_id;

-- استخدامها (يحسب في كل مرة)
SELECT * FROM employee_summary;

-- 2) إنشاء materialized view
CREATE MATERIALIZED VIEW department_stats AS
SELECT 
    d.id,
    d.name,
    COUNT(e.id) as emp_count,
    AVG(e.salary) as avg_salary
FROM departments d
LEFT JOIN employees e ON d.id = e.department_id
GROUP BY d.id, d.name;

-- استخدامها (سريع جداً، البيانات مخزّنة)
SELECT * FROM department_stats;
```

*مثال كامل:*

```sql
-- إنشاء materialized view
CREATE MATERIALIZED VIEW department_stats AS
SELECT 
    department_id,
    COUNT(*) as emp_count,
    AVG(salary) as avg_salary
FROM employees
GROUP BY department_id;

-- عرض النتائج
SELECT * FROM department_stats;

-- بعد إضافة موظفين جدد
INSERT INTO employees (name, department_id, salary) VALUES ('أحمد', 1, 5000);

-- النتائج قديمة الآن! ثم تحدثها
REFRESH MATERIALIZED VIEW department_stats;

-- الآن البيانات محدثة
SELECT * FROM department_stats;
```

*نقاط إضافية:*

- يمكن استخدام `REFRESH MATERIALIZED VIEW CONCURRENTLY` لعدم حجب الاستعلامات أثناء التحديث (يتطلب `UNIQUE INDEX`)
- في الممارسة العملية: جدول `REFRESH` تلقائياً بـ `scheduled tasks`/`cron jobs`

##### Phase 4: Advanced Features - المرحلة 4: الميزات المتقدمة

###### Stored Procedures and Functions

```sql
-- دالة بسيطة
--  عدد الموظفين في قسم معيّن
CREATE OR REPLACE FUNCTION get_employee_count(dept_id INTEGER)  -- ينشئ (أو يستبدل إن وجدت) دالة اسمها get_employee_count وتستقبل معاملًا واحدًا dept_id من النوع INTEGER. (رقم القسم الموضوع لمعرفة عدد موظفيه)

RETURNS INTEGER AS $$  -- الدالة ترجع قيمة واحدة من النوع INTEGER (عدد الموظفين).

-- AS $$ ... $$ LANGUAGE plpgsql;  -> جسم الدالة مكتوب بلغة PL/pgSQL ومحاط بـ $$ كـ delimiter.
DECLARE  -- يعرّف متغيرًا محليًا لتخزين الناتج المؤقت.
    count_result INTEGER;
BEGIN
    SELECT COUNT(*) INTO count_result
    FROM employees 
    WHERE department_id = dept_id;  -- يحسب عدد الصفوف في جدول employees التي عمود department_id يساوي قيمة المعامل dept_id، ويضع النتيجة في المتغير count_result.
    
    RETURN count_result;  -- يرجع القيمة المحسوبة كقيمة الدالة.
END;
$$ LANGUAGE plpgsql;

-- استخدام الدالة
SELECT get_employee_count(1);  -- يعيد عدد الموظفين في القسم رقم 1

-- يمكن تبسيطها بلغة SQL بدون متغير:
CREATE OR REPLACE FUNCTION get_employee_count(dept_id INTEGER)
RETURNS INTEGER AS $$
  SELECT COUNT(*) FROM employees WHERE department_id = $1;
$$ LANGUAGE sql;

-- دالة بإرجاع جدول
CREATE OR REPLACE FUNCTION get_department_employees(dept_id INTEGER)  -- ينشئ دالة اسمها get_department_employees تستقبل معامل dept_id من النوع INTEGER

RETURNS TABLE (
    emp_id INTEGER,
    emp_name VARCHAR,
    emp_salary DECIMAL
) AS $$
-- الدالة ترجع جدول (table) بثلاثة أعمدة:
-- emp_id: رقم الموظف
-- emp_name: اسم الموظف
-- emp_salary: راتب الموظف

BEGIN
    RETURN QUERY  -- يُرجع النتائج صفاً تلو الآخر
    SELECT id, first_name || ' ' || last_name, salary
    -- first_name || ' ' || last_name: يدمج الاسم الأول والأخير بمسافة بينهما
    FROM employees
    WHERE department_id = dept_id;
END;
$$ LANGUAGE plpgsql;

-- استخدام الدالة مثل جدول عادي
SELECT * FROM get_department_employees(1);

-- أو اختر أعمدة معينة
SELECT emp_name, emp_salary 
FROM get_department_employees(1) 
WHERE emp_salary > 5000;

-- يمكن تبسيطها بـ SQL بدون PL/pgSQL:
CREATE OR REPLACE FUNCTION get_department_employees(dept_id INTEGER)
RETURNS TABLE (emp_id INTEGER, emp_name VARCHAR, emp_salary DECIMAL) AS $$
  SELECT id, first_name || ' ' || last_name, salary
  FROM employees
  WHERE department_id = $1;
$$ LANGUAGE sql;
```

###### Triggers

- `Triggers - المشغلات`: هي إجراءات أو دوال تُنفَّذ تلقائيًا عند حدوث حدث معين في قاعدة البيانات، مثل عمليات `INSERT` أو `UPDATE` أو `DELETE`.

**أنواع Triggers:**

1. حسب وقت التنفيذ:
    - *BEFORE*: تنفذ قبل تنفيذ العملية
    - *AFTER*: تنفذ بعد تنفيذ العملية
    - *INSTEAD OF*: تنفذ بدلاً من العملية (لـ Views)

2. حسب مستوى التنفيذ:
    - *ROW-level*: تنفذ لكل صف متأثر
    - *STATEMENT-level*: تنفذ مرة واحدة لكل عملية

**بناء Trigger الأساسي:**

```sql
CREATE TRIGGER trigger_name
    {BEFORE | AFTER | INSTEAD OF} {event [OR ...]}
    ON table_name
    [FOR [EACH] {ROW | STATEMENT}]
    EXECUTE FUNCTION function_name();
```

**متغيرات خاصة في دوال Trigger:**

- *NEW*: الصف الجديد (لـ `INSERT` و `UPDATE`)
- *OLD*: الصف القديم (لـ `UPDATE` و `DELETE`)
- *TG_OP*: نوع العملية (`'INSERT'`, `'UPDATE'`, `'DELETE'`)
- *TG_TABLE_NAME*: اسم الجدول
- *TG_WHEN*: وقت التنفيذ (`'BEFORE'`, `'AFTER'`)

**إنشاء دالة Trigger:**

```sql
-- 1) إنشاء جدول السجل
CREATE TABLE audit_log (
    id SERIAL PRIMARY KEY,
    table_name VARCHAR,
    operation VARCHAR,
    old_data JSONB,
    new_data JSONB,
    changed_at TIMESTAMP
);

-- 2) إنشاء دالة trigger نموذجية
CREATE OR REPLACE FUNCTION log_changes()  -- تنشئ دالة اسمها log_changes
RETURNS TRIGGER AS $$  -- تُشير إلى أن هذه دالة trigger (ليست دالة عادية)
BEGIN
    IF TG_OP = 'INSERT' THEN
    -- TG_OP: متغير خاص يحتوي على نوع العملية (INSERT, UPDATE, DELETE)
    -- إذا كانت عملية إدراج، ينفّذ الكود التالي:
        INSERT INTO audit_log (table_name, operation, new_data, changed_at)
        VALUES (TG_TABLE_NAME, 'INSERT', row_to_json(NEW), now());
        RETURN NEW;
        -- TG_TABLE_NAME: اسم الجدول الذي حدثت عليه العملية
        -- NEW: الصف الجديد المُدرج
        -- row_to_json(NEW): تحويل الصف إلى JSON
        -- يسجل العملية في جدول audit_log للمراجعة

    ELSIF TG_OP = 'UPDATE' THEN  -- إذا كانت عملية تحديث:
        INSERT INTO audit_log (table_name, operation, old_data, new_data, changed_at)
        VALUES (TG_TABLE_NAME, 'UPDATE', row_to_json(OLD), row_to_json(NEW), now());  -- يسجل البيانات القديمة والجديدة
        RETURN NEW;
    
    ELSIF TG_OP = 'DELETE' THEN  -- إذا كانت عملية حذف:
        INSERT INTO audit_log (table_name, operation, old_data, changed_at)
        VALUES (TG_TABLE_NAME, 'DELETE', row_to_json(OLD), now());  -- يسجل البيانات المحذوفة
        RETURN OLD;
    END IF;
    
    RETURN NULL;
END;
$$ LANGUAGE plpgsql;

-- 3) ربط الـ trigger بالجدول
CREATE TRIGGER employees_audit_trigger
AFTER INSERT OR UPDATE OR DELETE ON employees
FOR EACH ROW
EXECUTE FUNCTION log_changes();

-- 4) الآن أي عملية على employees ستُسجل تلقائياً
INSERT INTO employees (name, salary) VALUES ('أحمد', 5000);
-- يُسجل تلقائياً في audit_log

UPDATE employees SET salary = 6000 WHERE name = 'أحمد';
-- يُسجل تحديث تلقائياً

DELETE FROM employees WHERE name = 'أحمد';
-- يُسجل حذف تلقائياً

-- 5) عرض السجلات
SELECT * FROM audit_log;
```

*الفائدة:*

- تدقيق البيانات: تسجيل من غيّر البيانات ومتى
- الاسترجاع: معرفة البيانات القديمة قبل التحديث
- الامتثال: تسجيل تغييرات لأغراض قانونية/تدقيق

**أمثلة عملية:**

*تسجيل التغييرات (Audit Trail):*

```sql
-- جدول للتسجيل
CREATE TABLE audit_log (
    id SERIAL PRIMARY KEY,
    table_name VARCHAR(100),
    operation VARCHAR(10),
    old_data JSONB,
    new_data JSONB,
    changed_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    changed_by VARCHAR(100)
);

-- إنشاء trigger
CREATE TRIGGER audit_employees
    AFTER INSERT OR UPDATE OR DELETE
    ON employees
    FOR EACH ROW
    EXECUTE FUNCTION log_changes();
```

*التحقق من البيانات قبل الإدخال:*

```sql
CREATE OR REPLACE FUNCTION validate_salary()
RETURNS TRIGGER AS $$
BEGIN
    IF NEW.salary < 0 THEN
        RAISE EXCEPTION 'الراتب لا يمكن أن يكون سالباً';
    END IF;
    
    IF NEW.salary > 1000000 THEN
        RAISE EXCEPTION 'الراتب كبير جداً';
    END IF;
    
    RETURN NEW;
END;
$$ LANGUAGE plpgsql;

CREATE TRIGGER validate_employee_salary
    BEFORE INSERT OR UPDATE
    ON employees
    FOR EACH ROW
    EXECUTE FUNCTION validate_salary();
```

*تحديث `timestamp` تلقائي:*

```sql
CREATE OR REPLACE FUNCTION update_timestamp()
RETURNS TRIGGER AS $$
BEGIN
    NEW.updated_at = CURRENT_TIMESTAMP;
    RETURN NEW;
END;
$$ LANGUAGE plpgsql;

CREATE TRIGGER update_employee_timestamp
    BEFORE UPDATE
    ON employees
    FOR EACH ROW
    EXECUTE FUNCTION update_timestamp();
```

*Maintaining Summary Tables:*

```sql
CREATE OR REPLACE FUNCTION update_order_summary()
RETURNS TRIGGER AS $$
BEGIN
    IF TG_OP = 'INSERT' THEN
        UPDATE order_summary 
        SET total_orders = total_orders + 1,
            total_amount = total_amount + NEW.amount
        WHERE customer_id = NEW.customer_id;
        
    ELSIF TG_OP = 'UPDATE' THEN
        UPDATE order_summary 
        SET total_amount = total_amount - OLD.amount + NEW.amount
        WHERE customer_id = NEW.customer_id;
        
    ELSIF TG_OP = 'DELETE' THEN
        UPDATE order_summary 
        SET total_orders = total_orders - 1,
            total_amount = total_amount - OLD.amount
        WHERE customer_id = OLD.customer_id;
    END IF;
    
    RETURN COALESCE(NEW, OLD);
END;
$$ LANGUAGE plpgsql;
```

**إدارة Triggers:**

*عرض Triggers الحالية:*

```sql
-- عرض جميع triggers
SELECT * FROM information_schema.triggers;

-- عرض triggers لجدول معين
SELECT trigger_name, event_manipulation, action_statement 
FROM information_schema.triggers 
WHERE event_object_table = 'employees';
```

*تعطيل/تمكين Trigger:*

```sql
-- تعطيل trigger
ALTER TABLE employees DISABLE TRIGGER audit_employees;

-- تمكين trigger
ALTER TABLE employees ENABLE TRIGGER audit_employees;
```

*حذف Trigger:*

```sql
DROP TRIGGER audit_employees ON employees;
```

**أفضل الممارسات:**

1. حافظ على بساطة دوال `Trigger`: تجنب العمليات المعقدة
2. استخدم للأتمتة فقط: لا تستخدم للبرمجة المنطقية المعقدة
3. كن حذراً مع الأداء: `Triggers` تؤثر على الأداء
4. توثيق `Triggers`: دوّن الغرض من كل `trigger`
5. اختبار شامل: اختبر جميع السيناريوهات الممكنة

**قيود ومحاذير:**

- لا يمكن استخدام `TRANSACTIONS` داخل `triggers`
- قد تؤدي إلى `deadlocks` إذا لم تُصمم بعناية
- صعوبة في التصحيح (`debugging`)
- قد تؤثر على الأداء في الجداول الكبيرة

###### JSONB والبيانات شبه المنظمة

```sql
-- إنشاء جدول بـ JSONB
CREATE TABLE products (
    id SERIAL PRIMARY KEY,
    name VARCHAR(200) NOT NULL,
    attributes JSONB,
    tags TEXT[],
    created_at TIMESTAMP DEFAULT NOW()
);

-- إدراج بيانات JSON
INSERT INTO products (name, attributes, tags) VALUES
('لابتوب', 
 '{"brand": "Dell", "ram": 16, "storage": 512, "screen": "15.6"}',
 '{"تقنية", "لابتوب", "أجهزة"}');

-- الاستعلام على JSONB
SELECT name, attributes->>'brand' as brand
FROM products 
WHERE attributes->>'brand' = 'Dell';

-- البحث في JSONB
SELECT name 
FROM products 
WHERE attributes @> '{"ram": 16}';

-- الفهارس على JSONB
CREATE INDEX idx_products_attributes ON products USING GIN(attributes);
CREATE INDEX idx_products_tags ON products USING GIN(tags);
```

###### Full-Text Search

بحث ذكي في النصوص يشبه محركات البحث الحديثة (مثل `Google`)

**الفرق بين البحث العادي والبحث الذكي:**

```sql
-- ❌ البحث العادي (محدود)
SELECT * FROM articles 
WHERE content LIKE '%برمجة%';

-- ✅ البحث الذكي (متقدم)
SELECT * FROM articles 
WHERE to_tsvector('arabic', content) @@ to_tsquery('برمجة & قواعد');
```

**كيف يعمل Full-Text Search؟:**

*الخطوات الأساسية:*

1. تحويل النص إلى `tsvector` (تفكيك النص إلى كلمات أساسية)
2. تحويل كلمة البحث إلى `tsquery` (صيغة استعلام بحث)
3. المقارنة بينهما باستخدام `@@`

**التطبيق العملي خطوة بخطوة:**

*الخطوة 1: إنشاء جدول تجريبي:*

```sql
CREATE TABLE articles (
    id SERIAL PRIMARY KEY,
    title VARCHAR(500) NOT NULL,
    content TEXT,
    author VARCHAR(100),
    created_at TIMESTAMP DEFAULT NOW()
);

-- إدراج بيانات مثالبة
INSERT INTO articles (title, content, author) VALUES
('تعلم البرمجة مع PostgreSQL', 'هذا المقال يتناول أساسيات البرمجة وقواعد البيانات باستخدام PostgreSQL مع أمثلة عملية', 'أحمد'),
('أفضل ممارسات قواعد البيانات', 'دليل شامل لأفضل الممارسات في تصميم قواعد البيانات وتحسين الأداء مع نصائح عملية', 'فاطمة'),
('الذكاء الاصطناعي وتطبيقاته', 'استكشاف عالم الذكاء الاصطناعي وتطبيقاته في تحليل البيانات والتعلم الآلي', 'خالد');
```

*الخطوة 2: البحث الأساسي بدون فهارس:*

```sql
-- بحث بسيط (بدون تحضير مسبق)
SELECT title, content
FROM articles
WHERE to_tsvector('arabic', title || ' ' || content) @@ to_tsquery('arabic', 'برمجة');
-- 'arabic': اللغة - اختياري لكن مستحب
-- title || ' ' || content: دمج العنوان والمحتوى في نص واحد
-- @@: عامل المطابقة (هل يتطابق tsvector مع tsquery؟)
-- to_tsquery('arabic', 'برمجة'): تحويل كلمة البحث إلى استعلام

-- أو بشكل منفصل
SELECT title, content
FROM articles
WHERE to_tsvector('arabic', title) @@ to_tsquery('arabic', 'برمجة')
   OR to_tsvector('arabic', content) @@ to_tsquery('arabic', 'برمجة');
```

**الطريقة المحسنة (باستخدام أعمدة مخزنة وفهارس):**

*الخطوة 3: إضافة عمود `tsvector` وفحص GIN:*

```sql
-- إضافة عمود مخزن لـ tsvector
ALTER TABLE articles ADD COLUMN search_vector tsvector;

-- تحديث العمود بالبيانات
UPDATE articles SET search_vector = 
    to_tsvector('arabic', coalesce(title, '') || ' ' || coalesce(content, ''));
-- coalesce(column, ''): إذا كان العمود NULL، استبدله بسطر فارغ ''
-- السبب: تجنب NULL الذي قد يسبب أخطاء في الدمج
-- مثلا إذا كان title = NULL و content = 'النص'
-- بدون coalesce: NULL || ' ' || 'النص' = NULL
-- مع coalesce: '' || ' ' || 'النص' = ' النص'

-- إنشاء فهرس GIN (سريع جداً للبحث)
CREATE INDEX idx_articles_search ON articles USING gin(search_vector);
-- GIN = Generalized Inverted Index - مصمم خصيصاً للبحث النصي
```

*الخطوة 4: البحث باستخدام الفهرس:*

```sql
-- بحث سريع باستخدام الفهرس
SELECT title, content
FROM articles
WHERE search_vector @@ to_tsquery('PostgreSQL');
```

**التحديث التلقائي باستخدام Triggers:**

*الخطوة 5: جعل البحث ديناميكي:*

```sql
-- إنشاء دالة للتحديث التلقائي
CREATE OR REPLACE FUNCTION articles_search_vector_update()
RETURNS TRIGGER AS $$
BEGIN
    NEW.search_vector = to_tsvector('arabic',
        coalesce(NEW.title, '') || ' ' || coalesce(NEW.content, ''));
    RETURN NEW;
END;
$$ LANGUAGE plpgsql;

-- إنشاء التريجر
CREATE TRIGGER tsvector_update_trigger
    BEFORE INSERT OR UPDATE ON articles
    FOR EACH ROW
    EXECUTE FUNCTION articles_search_vector_update();
```

**صيغ البحث المتقدمة في `to_tsquery`:**

*أنواع الاستعلامات:*

```sql
-- البحث بكلمة واحدة
SELECT * FROM articles 
WHERE search_vector @@ to_tsquery('arabic', 'برمجة');

-- البحث بـ AND (&)
SELECT * FROM articles 
WHERE search_vector @@ to_tsquery('arabic', 'برمجة & قواعد');

-- البحث بـ OR (|)
SELECT * FROM articles 
WHERE search_vector @@ to_tsquery('arabic', 'برمجة | ذكاء');

-- البحث بـ NOT (!)
SELECT * FROM articles 
WHERE search_vector @@ to_tsquery('arabic', 'برمجة & !جافا');

-- البحث بعبارة (باستخدام <-> للمجاورة)
SELECT * FROM articles 
WHERE search_vector @@ to_tsquery('arabic', 'قواعد <-> البيانات');
-- to_tsquery('arabic', 'قواعد البيانات') -> ERROR

-- البحث باستخدام wildcard (:*)
SELECT * FROM articles 
WHERE search_vector @@ to_tsquery('arabic', 'برمج:*');
```

**ترتيب النتائج حسب الأهمية:**

*استخدام `ts_rank` للترتيب:*

```sql
SELECT 
    title,
    content,
    ts_rank(search_vector, to_tsquery('arabic', 'برمجة | قواعد')) as rank
FROM articles
WHERE search_vector @@ to_tsquery('arabic', 'برمجة | قواعد')
ORDER BY rank DESC;
```

*ترتيب متقدم مع أوزان:*

- معنى الأوزان `{A, B, C, D}`:
  - `A = 0.1`: وزن الكلمات المهملة (the, a, is)
  - `B = 0.2`: وزن الكلمات غير المهمة
  - `C = 0.4`: وزن الكلمات العادية
  - `D = 1.0`: وزن الكلمات المهمة (في العناوين عادة)

```sql
SELECT 
    title,
    content,
    ts_rank(
        '{0.1, 0.2, 0.4, 1.0}',  -- أوزان: العنوان أهم من المحتوى
        search_vector,
        to_tsquery('arabic', 'برمجة')
    ) as rank
FROM articles
WHERE search_vector @@ to_tsquery('arabic', 'برمجة')
ORDER BY rank DESC;
```

**دعم اللغات (بما فيها العربية):**

*اللغات المدعومة:*

```sql
-- عرض اللغات المدعومة
SELECT cfgname FROM pg_ts_config;

-- لغات شائعة:
to_tsvector('english', text)    -- الإنجليزية
to_tsvector('arabic', text)     -- العربية ✅
to_tsvector('simple', text)     -- بسيط (بدون معالجة لغوية)
```

**مثال متكامل لنظام بحث:**

*نظام بحث متكامل للمدونة:*

```sql
-- إنشاء الجدول مع البحث
CREATE TABLE blog_posts (
    id SERIAL PRIMARY KEY,
    title VARCHAR(500) NOT NULL,
    content TEXT NOT NULL,
    tags TEXT[],
    search_vector tsvector,
    created_at TIMESTAMP DEFAULT NOW()
);

-- الفهرس
CREATE INDEX idx_blog_search ON blog_posts USING gin(search_vector);

-- التريجر للتحديث التلقائي
CREATE TRIGGER blog_search_update
    BEFORE INSERT OR UPDATE ON blog_posts
    FOR EACH ROW EXECUTE FUNCTION articles_search_vector_update();

-- دالة بحث متقدمة
CREATE OR REPLACE FUNCTION search_blog(query TEXT)
RETURNS TABLE (
    post_id INTEGER,
    post_title VARCHAR,
    post_content TEXT,
    relevance REAL
) AS $$
BEGIN
    RETURN QUERY
    SELECT 
        bp.id,
        bp.title,
        substring(bp.content from 1 for 200) || '...' as excerpt,  -- خذ أول 200 حرف من المحتوى وأضف نقاط (...) للإشارة أن النص مقصوص
        ts_rank(bp.search_vector, to_tsquery('arabic', query)) as rank
    FROM blog_posts bp
    WHERE bp.search_vector @@ to_tsquery('arabic', query)
    ORDER BY rank DESC;
END;
$$ LANGUAGE plpgsql;

-- استخدام دالة البحث
SELECT * FROM search_blog('برمجة & قواعد');
```

**نصائح أداء مهمة:**

*لتحسين الأداء:*

```sql
-- 1. استخدام الفهرس GIN
CREATE INDEX idx_search ON table USING gin(tsvector_column);

-- 2. تقسيم النص الكبير
WHERE search_vector @@ to_tsquery('كلمة')
AND length(content) < 10000;  -- تجنب النصوص الطويلة جداً

-- 3. تحديث الإحصائيات
ANALYZE table_name;
```

**الخلاصة: متى تستخدم Full-Text Search؟:**

*استخدمه عندما تحتاج:*

- بحث في مقالات، مدونات، محتوى
- نظام بحث في موقعك
- بحث ذكي في نصوص طويلة
- ترتيب النتائج حسب الأهمية

*لا تستخدمه عندما:*

- تبحث في أرقام أو تواريخ
- تبحث في كلمات دقيقة (استخدم `=` أو `LIKE`)
- البيانات صغيرة جداً

**مثال نهائي:**

```sql
-- إعداد البحث النصي
CREATE TABLE articles (
    id SERIAL PRIMARY KEY,
    title VARCHAR(500) NOT NULL,
    content TEXT,
    author VARCHAR(100),
    search_vector tsvector,
    created_at TIMESTAMP DEFAULT NOW()
);

-- إنشاء الفهرس
CREATE INDEX idx_articles_search ON articles USING GIN(search_vector);

-- تحديث search vector
UPDATE articles SET search_vector = 
    to_tsvector('arabic', coalesce(title, '') || ' ' || coalesce(content, ''));

-- أو استخدام Trigger للتحديث التلقائي
CREATE OR REPLACE FUNCTION articles_search_vector_update()
RETURNS TRIGGER AS $$
BEGIN
    NEW.search_vector = to_tsvector('arabic', 
        coalesce(NEW.title, '') || ' ' || coalesce(NEW.content, ''));
    RETURN NEW;
END;
$$ LANGUAGE plpgsql;

CREATE TRIGGER tsvector_update_trigger
    BEFORE INSERT OR UPDATE ON articles
    FOR EACH ROW
    EXECUTE FUNCTION articles_search_vector_update();

-- البحث
SELECT title, content
FROM articles
WHERE search_vector @@ to_tsquery('arabic', 'برمجة & قواعد');

-- البحث مع الترتيب حسب الأهمية
SELECT title, 
       ts_rank(search_vector, to_tsquery('arabic', 'برمجة')) as rank
FROM articles
WHERE search_vector @@ to_tsquery('arabic', 'برمجة')
ORDER BY rank DESC;
```

###### Administration and Security - الإدارة والأمان

**إدارة المستخدمين والصلاحيات:**

*إنشاء مستخدمين جديدين:*

```sql
-- إنشاء مستخدم عادي
CREATE USER app_user WITH PASSWORD 'secure_password_123';

-- إنشاء مستخدم مع صلاحيات محددة
CREATE USER developer WITH 
    PASSWORD 'dev_pass'
    VALID UNTIL '2024-12-31';  -- يجعل كلمة المرور تنتهي في تاريخ محدد (مفيد للمستخدمين المؤقتين أو المتدربين)

-- في التطبيق، تستخدم هذا الاسم للاتصال:
-- في كود Python
-- conn = psycopg2.connect(
--     host="localhost",
--     user="app_user",  # هذا الذي أنشأته
--     password="secure_password_123",
--     database="my_db"
-- )
```

*إدارة المجموعات والأدوار:*

```sql
-- إنشاء مجموعة
CREATE ROLE read_only;
CREATE ROLE read_write;

-- منح صلاحيات للمجموعات
GRANT SELECT ON ALL TABLES IN SCHEMA public TO read_only;
GRANT SELECT, INSERT, UPDATE ON ALL TABLES IN SCHEMA public TO read_write;

-- إضافة مستخدم للمجموعة
GRANT read_write TO app_user;
```

**الصلاحيات على قواعد البيانات والجداول:**

*الصلاحيات الأساسية:*

```sql
-- منح صلاحيات على قاعدة بيانات
GRANT CONNECT ON DATABASE company TO app_user;

-- منح صلاحيات على schema
GRANT USAGE ON SCHEMA public TO app_user;

-- منح صلاحيات على جداول محددة
GRANT SELECT, INSERT, UPDATE ON users TO app_user;
GRANT SELECT ON products TO app_user;

-- منح كل الصلاحيات على جدول
GRANT ALL PRIVILEGES ON orders TO developer;
```

*إلغاء الصلاحيات:*

```sql
-- إلغاء صلاحيات
REVOKE INSERT ON users FROM app_user;
REVOKE ALL ON orders FROM developer;
```

**الأمان - الحماية من الهجمات الشائعة:**

*الحماية من SQL Injection:*

```python
# الطريقة الخطأ (عرضة للهجوم):
query = f"SELECT * FROM users WHERE username = '{user_input}'"  # خطير - عرضة لـ SQL Injection

# الطريقة الصحيحة (آمنة):
query = "SELECT * FROM users WHERE username = %s"  # آمن - استخدام المعلمات
cursor.execute(query, (user_input,))

# في Node.js
# const query = 'SELECT * FROM users WHERE username = $1';
# const result = await pool.query(query, [username]);
```

*إعدادات الأمان في postgresql.conf:*

- إعدادات أمان مهمة:

```conf
# في ملف postgresql.conf

# تقييد عناوين IP المسموح بها
listen_addresses = 'localhost, 192.168.1.100'

# تشفير الاتصالات
ssl = on

# وقت انتهاء كلمة المرور
password_encryption = scram-sha-256

# الحد الأقصى للمحاولات الفاشلة
max_connections = 100
```

*المصادقة في pg_hba.conf:*

- ضبط طرق المصادقة:

```conf
# في ملف pg_hba.conf

# مصادقة كلمة مرور مشفرة للمستخدمين المحليين
local   all             all                                     scram-sha-256

# مصادقة من شبكة محلية
host    all             all             192.168.1.0/24          scram-sha-256

# رفض الاتصالات من خارج الشبكة
host    all             all             0.0.0.0/0               reject
```

**المهام الإدارية اليومية:**

*النسخ الاحتياطي (Backup):*

- ما ينسخ: كل الجداول، البيانات، العلاقات، الفهارس
- لماذا: لحماية البيانات من الضياع
- متى: عند التحديثات الكبيرة، تغيير السيرفر، نسخ للبيئة التطويرية
- متى تستخدم الاستعادة:
  - عندما يحذف أحدهم بيانات بالخطأ
  - عند تجربة `feature` جديد وفشل
  - لنسخ بيانات `Production` إلى `Development`

```bash
# نسخ كامل
pg_dump -U postgres -h localhost company > backup.sql

# نسخ مضغوط
pg_dump -U postgres -Fc company > backup.dump

# نسخ مع استبعاد جداول معينة
pg_dump -U postgres -T temp_logs company > backup.sql

# -----------------

# استعادة من نسخ SQL
psql -U postgres -d company < backup.sql

# استعادة من نسخ مضغوط
pg_restore -U postgres -d company backup.dump
```

*المراقبة والأداء:*

```sql
-- قد يتطلب بعض الإعدادات الخاصة
-- عرض الاستعلامات النشطة
SELECT * FROM pg_stat_activity;

-- عرض الاستعلامات البطيئة
SELECT query, total_time 
FROM pg_stat_statements 
ORDER BY total_time DESC 
LIMIT 10;

-- عرض حجم الجداول
SELECT 
    table_name,
    pg_size_pretty(pg_total_relation_size(table_name)) as size
FROM information_schema.tables 
WHERE table_schema = 'public';
```

*إحصائيات الأداء:*

```sql
-- فحص واستعادة الإحصائيات
ANALYZE;

-- تنظيف وتحسين الجداول
VACUUM ANALYZE users;

-- إعادة بناء الفهارس
REINDEX TABLE orders;
```

**أفضل ممارسات الأمان للمطورين:**

*مبادئ الامتيازات الدنيا:*

```sql
-- ❌ خطأ - منح كل الصلاحيات
GRANT ALL PRIVILEGES ON DATABASE company TO app_user;

-- ✅ صحيح - منح الصلاحيات المحددة فقط
GRANT CONNECT ON DATABASE company TO app_user;
GRANT SELECT ON public.products TO app_user;
GRANT INSERT ON public.orders TO app_user;
```

*فصل الصلاحيات حسب الوظيفة:*

```sql
-- مستخدم للتطبيق
CREATE USER app_user WITH PASSWORD 'app_pass';
GRANT SELECT, INSERT, UPDATE ON users, orders TO app_user;

-- مستخدم للتقارير
CREATE USER reporter WITH PASSWORD 'report_pass';
GRANT SELECT ON users, orders, products TO reporter;

-- مستخدم للإدارة
CREATE USER admin_user WITH PASSWORD 'admin_pass';
GRANT ALL PRIVILEGES ON ALL TABLES IN SCHEMA public TO admin_user;
```

*مراقبة الأمان:*

```sql
-- تفعيل تسجيل الاستعلامات البطيئة
ALTER SYSTEM SET log_min_duration_statement = '1000ms';
-- سجل أي استعلام يستغرق أكثر من ثانية

-- تسجيل محاولات الدخول الفاشلة
ALTER SYSTEM SET log_connections = on;
-- سجل كل من يتصل بقاعدة البيانات

ALTER SYSTEM SET log_disconnections = on;

-- إعادة تحميل الإعدادات
SELECT pg_reload_conf();
-- طبق التغييرات دون إعادة تشغيل الخادم
```

**نصوص مساعدة للإدارة:**

*نص لمراقبة الأداء:*

```sql
-- عرض أكبر 10 جداول
SELECT 
    schemaname,
    tablename,
    pg_size_pretty(pg_total_relation_size(schemaname||'.'||tablename)) as size
FROM pg_tables 
WHERE schemaname NOT IN ('information_schema', 'pg_catalog')
ORDER BY pg_total_relation_size(schemaname||'.'||tablename) DESC
LIMIT 10;
```

*نص لمراقبة المستخدمين:*

```sql
-- عرض جميع المستخدمين وصلاحياتهم
SELECT 
    usename as username,
    usesuper as is_superuser,
    usecreatedb as can_create_db
FROM pg_user;
```

*نص للنسخ الاحتياطي التلقائي:*

```bash
#!/bin/bash
# script: backup.sh
DATE=$(date +%Y-%m-%d_%H-%M-%S)
pg_dump -U postgres company > /backups/company_$DATE.sql
find /backups -name "company_*.sql" -mtime +7 -delete
```

**التكامل مع التطبيقات:**

*إعداد اتصال آمن من التطبيق:*

```python
# Python مع إعدادات أمان
import psycopg2

def get_db_connection():
    return psycopg2.connect(
        host="localhost",
        database="company",
        user="app_user",  # مستخدم محدود الصلاحيات
        password="secure_password",
        port=5432,
        # إعدادات أمان إضافية
        sslmode="require",  # تشفير الاتصال
        connect_timeout=10   # مهلة اتصال
    )
```

*إدارة الاتصالات في Node.js:*

```javascript
// إعداد pool مع حد أقصى للاتصالات
const { Pool } = require('pg');

const pool = new Pool({
    user: 'app_user',
    host: 'localhost',
    database: 'company',
    password: 'secure_password',
    port: 5432,
    max: 20, // الحد الأقصى للاتصالات
    idleTimeoutMillis: 30000,
    connectionTimeoutMillis: 2000,
});
```

**الخلاصة: ما تحتاجه كمطور Backend:**

*إجباري:*

- إنشاء وإدارة المستخدمين
- منح الصلاحيات المناسبة
- الحماية من `SQL Injection`
- النسخ الاحتياطي الأساسي

*مستحب:*

- مراقبة الأداء
- فهم إعدادات الأمان
- إدارة الاتصالات

*متقدم (للمسؤولين):*

- إعدادات الخادم المتقدمة
- التشفير المتقدم
- النسخ الاحتياطي التلقائي

**مثال كامل:**

```sql
-- إدارة المستخدمين
CREATE USER app_user WITH PASSWORD 'secure_password_123';
CREATE ROLE read_only;
CREATE ROLE read_write;

-- الصلاحيات
GRANT CONNECT ON DATABASE company TO app_user;
GRANT USAGE ON SCHEMA public TO app_user;

-- صلاحيات محددة
GRANT SELECT ON employees TO read_only;
GRANT SELECT, INSERT, UPDATE ON employees TO read_write;

-- منح الأدوار
GRANT read_write TO app_user;

-- النسخ الاحتياطي
-- من سطر الأوامر:
pg_dump company > backup.sql
pg_dump -Fc company > backup.dump  -- نسخ مضغوط

-- الاستعادة
psql company < backup.sql
pg_restore -d company backup.dump
```

##### Phase 5: Integration with Applications - المرحلة 5: التكامل مع التطبيقات

###### التكامل مع Node.js

```javascript
// package.json
{
  "dependencies": {
    "pg": "^8.11.0",
    "pg-pool": "^3.6.0"
  }
}

// db.js
const { Pool } = require('pg');

const pool = new Pool({
  user: 'app_user',
  host: 'localhost',
  database: 'company',
  password: 'password',
  port: 5432,
  max: 20, // maximum number of clients in the pool
  idleTimeoutMillis: 30000,
  connectionTimeoutMillis: 2000,
});

// استعلام بسيط
async function getEmployees() {
  const client = await pool.connect();
  try {
    const result = await client.query('SELECT * FROM employees');
    return result.rows;
  } finally {
    client.release();
  }
}

// استعلام مع معلمات
async function getEmployeeById(id) {
  const result = await pool.query(
    'SELECT * FROM employees WHERE id = $1',
    [id]
  );
  return result.rows[0];
}

// معاملة
async function transferSalary(fromAccount, toAccount, amount) {
  const client = await pool.connect();
  try {
    await client.query('BEGIN');
    
    await client.query(
      'UPDATE accounts SET balance = balance - $1 WHERE id = $2',
      [amount, fromAccount]
    );
    
    await client.query(
      'UPDATE accounts SET balance = balance + $1 WHERE id = $2',
      [amount, toAccount]
    );
    
    await client.query('COMMIT');
  } catch (error) {
    await client.query('ROLLBACK');
    throw error;
  } finally {
    client.release();
  }
}

module.exports = { pool, getEmployees, getEmployeeById, transferSalary };
```

###### التكامل مع Python

```python
# requirements.txt
# psycopg2-binary==2.9.6

import psycopg2
from psycopg2 import pool

# Connection Pool
connection_pool = psycopg2.pool.SimpleConnectionPool(
    1, 20,
    user="app_user",
    password="password",
    host="localhost",
    port="5432",
    database="company"
)

def get_employees():
    conn = connection_pool.getconn()
    try:
        with conn.cursor() as cur:
            cur.execute("SELECT * FROM employees")
            return cur.fetchall()
    finally:
        connection_pool.putconn(conn)

def get_employee_by_id(employee_id):
    conn = connection_pool.getconn()
    try:
        with conn.cursor() as cur:
            cur.execute(
                "SELECT * FROM employees WHERE id = %s",
                (employee_id,)
            )
            return cur.fetchone()
    finally:
        connection_pool.putconn(conn)

# استخدام with للتعامل الآمن
def create_employee(first_name, last_name, email, salary):
    conn = connection_pool.getconn()
    try:
        with conn.cursor() as cur:
            cur.execute(
                """INSERT INTO employees 
                (first_name, last_name, email, salary) 
                VALUES (%s, %s, %s, %s) RETURNING id""",
                (first_name, last_name, email, salary)
            )
            new_id = cur.fetchone()[0]
            conn.commit()
            return new_id
    except Exception as e:
        conn.rollback()
        raise e
    finally:
        connection_pool.putconn(conn)
```

###### التكامل مع Java

```java
// Maven: pom.xml
/*
<dependency>
    <groupId>org.postgresql</groupId>
    <artifactId>postgresql</artifactId>
    <version>42.6.0</version>
</dependency>
*/

import java.sql.*;
import javax.sql.DataSource;
import org.postgresql.ds.PGSimpleDataSource;

public class PostgreSQLConnection {
    private DataSource dataSource;
    
    public PostgreSQLConnection() {
        PGSimpleDataSource ds = new PGSimpleDataSource();
        ds.setServerName("localhost");
        ds.setDatabaseName("company");
        ds.setUser("app_user");
        ds.setPassword("password");
        ds.setPortNumber(5432);
        this.dataSource = ds;
    }
    
    public void getEmployees() throws SQLException {
        String sql = "SELECT id, first_name, last_name, salary FROM employees";
        
        try (Connection conn = dataSource.getConnection();
             PreparedStatement pstmt = conn.prepareStatement(sql);
             ResultSet rs = pstmt.executeQuery()) {
            
            while (rs.next()) {
                System.out.printf("ID: %d, Name: %s %s, Salary: %.2f%n",
                    rs.getInt("id"),
                    rs.getString("first_name"),
                    rs.getString("last_name"),
                    rs.getDouble("salary"));
            }
        }
    }
    
    public int createEmployee(String firstName, String lastName, 
                            String email, double salary) throws SQLException {
        String sql = "INSERT INTO employees (first_name, last_name, email, salary) VALUES (?, ?, ?, ?) RETURNING id";
        
        try (Connection conn = dataSource.getConnection();
             PreparedStatement pstmt = conn.prepareStatement(sql)) {
            
            pstmt.setString(1, firstName);
            pstmt.setString(2, lastName);
            pstmt.setString(3, email);
            pstmt.setDouble(4, salary);
            
            ResultSet rs = pstmt.executeQuery();
            if (rs.next()) {
                return rs.getInt(1);
            }
            throw new SQLException("Failed to get generated ID");
        }
    }
}
```

###### أفضل الممارسات والأمان

**أفضل الممارسات:**

```sql
-- 1. استخدم المعلمات دائماً
-- سيء (عرضة لـ SQL Injection)
SELECT * FROM users WHERE username = '" + username + "';

-- جيد (آمن)
SELECT * FROM users WHERE username = $1;

-- 2. استخدم الفهارس بحكمة
CREATE INDEX idx_optimized ON table (col1, col2) WHERE condition;

-- 3. مراقبة الأداء
SELECT * FROM pg_stat_activity;  -- النشاط الحالي
SELECT * FROM pg_stat_user_tables; -- إحصائيات الجداول

-- 4. الصيانة الدورية
VACUUM ANALYZE;  -- تنظيف وتحليل الإحصائيات
REINDEX TABLE table_name; -- إعادة بناء الفهارس
```

**إعدادات مهمة في postgresql.conf:**

```conf
shared_buffers = 25% of RAM
work_mem = 50MB
maintenance_work_mem = 512MB
effective_cache_size = 75% of RAM
```

###### مشروع نهائي متكامل

**مشروع نظام إدارة الموظفين:**

```sql
-- هيكل قاعدة البيانات
CREATE TABLE departments (
    id SERIAL PRIMARY KEY,
    name VARCHAR(100) NOT NULL UNIQUE,
    budget DECIMAL(12,2),
    created_at TIMESTAMP DEFAULT NOW()
);

CREATE TABLE employees (
    id SERIAL PRIMARY KEY,
    first_name VARCHAR(50) NOT NULL,
    last_name VARCHAR(50) NOT NULL,
    email VARCHAR(100) UNIQUE NOT NULL,
    phone VARCHAR(20),
    salary DECIMAL(10,2) CHECK (salary > 0),
    hire_date DATE NOT NULL,
    department_id INTEGER REFERENCES departments(id),
    manager_id INTEGER REFERENCES employees(id),
    is_active BOOLEAN DEFAULT true,
    created_at TIMESTAMP DEFAULT NOW()
);

CREATE TABLE projects (
    id SERIAL PRIMARY KEY,
    name VARCHAR(200) NOT NULL,
    description TEXT,
    budget DECIMAL(12,2),
    start_date DATE,
    end_date DATE,
    department_id INTEGER REFERENCES departments(id),
    status VARCHAR(20) DEFAULT 'active'
);

CREATE TABLE employee_projects (
    employee_id INTEGER REFERENCES employees(id),
    project_id INTEGER REFERENCES projects(id),
    role VARCHAR(50),
    assigned_date DATE DEFAULT CURRENT_DATE,
    PRIMARY KEY (employee_id, project_id)
);

-- Views مفيدة
CREATE VIEW employee_summary AS
SELECT 
    e.id,
    e.first_name || ' ' || e.last_name as full_name,
    e.email,
    e.salary,
    d.name as department_name,
    COUNT(ep.project_id) as project_count
FROM employees e
LEFT JOIN departments d ON e.department_id = d.id
LEFT JOIN employee_projects ep ON e.id = ep.employee_id
WHERE e.is_active = true
GROUP BY e.id, e.first_name, e.last_name, e.email, e.salary, d.name;

-- دوال مساعدة
CREATE OR REPLACE FUNCTION get_department_employees(dept_name VARCHAR)
RETURNS TABLE (
    employee_id INTEGER,
    full_name VARCHAR,
    salary DECIMAL,
    hire_date DATE
) AS $$
BEGIN
    RETURN QUERY
    SELECT 
        e.id,
        e.first_name || ' ' || e.last_name,
        e.salary,
        e.hire_date
    FROM employees e
    INNER JOIN departments d ON e.department_id = d.id
    WHERE d.name = dept_name AND e.is_active = true
    ORDER BY e.hire_date DESC;
END;
$$ LANGUAGE plpgsql;
```

##### Final Exam - اختبار نهائي

**أسئلة تقييمية:**

1. ما الفرق بين `INNER JOIN` و `LEFT JOIN`؟

2. متى تستخدم الفهرس الجزئي (`Partial Index`)؟

3. كيف تمنع هجمات `SQL Injection`؟

4. ما فائدة `Window Functions`؟

5. كيف تتعامل مع البيانات شبه المنظمة في `PostgreSQL`؟

6. ما الفرق بين `WHERE` و `HAVING` في الأداء؟

7. كيف يؤثر ترتيب الشروط على خطة التنفيذ؟

8. متى يستخدم الفهرس ومتى يتجاهله المحرك؟

9. أي شرط يوضع أولاً؟ ولماذا؟

    ```sql
    SELECT * FROM orders 
    WHERE customer_id = 123 
    AND order_date > '2023-01-01'
    AND status = 'shipped';
    ```

10. ما هي `snake_case` وكيف تستخدم في تسمية الجداول والأعمدة؟

11. ما هو `pg_stat_statements`؟

12. ما هو `Connection Pooling` المستخدم في الاتصالات المجمعة؟

13. ما هو `Query Optimization` عمليا؟

14. كيفية إدراج مليون صف بكفاءة؟

15. حل مشكلة متزامنة:
    - لديك عملية تحويل أموال:
        1. خصم من الحساب A
        2. إضافة للحساب B

    - كيف تضمن عدم فقدان الأموال عند حدوث خطأ؟

16. إذا كان لدي جدول `orders` به `customer_name` و `customer_phone` يتكرران في كل طلب، ما المشكلة وكيف أحلها؟

17. ماذا يحدث إذا فشلت العملية الثانية في تحويل الأموال بين حسابين؟ كيف أضمن عدم فقدان الأموال؟

**إجابات الأسئلة:**

1. الفرق بين `INNER JOIN` و `LEFT JOIN`

    ```sql
    -- INNER JOIN: النتائج المشتركة فقط
    SELECT users.name, orders.total
    FROM users
    INNER JOIN orders ON users.id = orders.user_id;
    -- النتيجة: فقط المستخدمين الذين لديهم طلبات

    -- LEFT JOIN: كل النتائج من الجدول الأيسر + المشتركة
    SELECT users.name, orders.total
    FROM users
    LEFT JOIN orders ON users.id = orders.user_id;
    -- النتيجة: كل المستخدمين، حتى بدون طلبات (orders.total يكون NULL)
    ```

    *الفرق:* `INNER JOIN` يعطي التقاطع فقط، `LEFT JOIN` يعطي كل البيانات من اليسار + التقاطع.

2. متى تستخدم الفهرس الجزئي (`Partial Index`)

    ```sql
    -- عندما تريد فهرس على جزء من البيانات فقط
    CREATE INDEX idx_active_users ON users(email) WHERE is_active = true;

    -- الاستخدام الأمثل:
    -- ✅ على البيانات النشطة فقط (active users)
    -- ✅ على الحالات الشائعة (status = 'completed')
    -- ✅ لتجنب فهرسة بيانات قديمة أو غير مهمة
    ```

    *الفائدة:* أداء أفضل ومساحة أقل.

3. منع هجمات `SQL Injection`

    ```python
    # ❌ خطير - عرضة للهجوم
    query = f"SELECT * FROM users WHERE username = '{user_input}'"

    # ✅ آمن - استخدام المعلمات
    query = "SELECT * FROM users WHERE username = %s"
    cursor.execute(query, (user_input,))

    # ✅ في Node.js
    const query = 'SELECT * FROM users WHERE username = $1';
    await pool.query(query, [username]);
    ```

    *الحل:* استخدم `Parameterized Queries` دائماً.

4. فائدة `Window Functions`

    ```sql
    -- إحصائيات بدون تجميع الصفوف
    SELECT 
        name,
        department,
        salary,
        AVG(salary) OVER (PARTITION BY department) as dept_avg,
        RANK() OVER (PARTITION BY department ORDER BY salary DESC) as rank
    FROM employees;
    -- النتيجة: كل صف فردي مع إحصائيات متعلقه
    ```

    *الفائدة:* تحليلات متقدمة دون فقدان التفاصيل الفردية.

5. التعامل مع البيانات شبه المنظمة

    ```sql
    -- استخدام JSONB
    CREATE TABLE products (
        id SERIAL PRIMARY KEY,
        name VARCHAR(100),
        attributes JSONB  -- {color: "red", size: "large", tags: ["new", "sale"]}
    );

    -- البحث في JSONB
    SELECT name FROM products 
    WHERE attributes @> '{"color": "red"}';

    -- الفهرس على JSONB
    CREATE INDEX idx_products_attrs ON products USING GIN(attributes);
    ```

6. الفرق بين `WHERE` و `HAVING` في الأداء

    ```sql
    -- WHERE: تصفية الصفوف قبل التجميع (أفضل أداء)
    SELECT department, AVG(salary)
    FROM employees
    WHERE salary > 5000          -- يطبق على كل صف فردي
    GROUP BY department;

    -- HAVING: تصفية النتائج بعد التجميع (أقل أداء)
    SELECT department, AVG(salary)
    FROM employees
    GROUP BY department
    HAVING AVG(salary) > 5000;   -- يطبق على المجموعات
    ```

    *الأداء:* `WHERE` أفضل لأنه يعمل على بيانات أقل.

7. تأثير ترتيب الشروط على خطة التنفيذ

    ```sql
    -- ❌ أقل كفاءة
    SELECT * FROM users 
    WHERE LOWER(name) = 'ahmed' 
    AND age > 25;

    -- ✅ أكثر كفاءة
    SELECT * FROM users 
    WHERE age > 25 
    AND LOWER(name) = 'ahmed';
    ```

    *السبب:* ضع الشروط الأكثر انتقائية أولاً لتقليل البيانات بسرعة.

8. متى يستخدم الفهرس ومتى يتجاهله

    ```sql
    -- ✅ يستخدم الفهرس
    WHERE email = 'test@example.com'          -- مساواة مباشرة
    WHERE id IN (1, 2, 3)                     -- قيم محددة
    WHERE created_at > '2023-01-01'           -- نطاق مرتب

    -- ❌ قد يتجاهل الفهرس
    WHERE LOWER(email) = 'test@example.com'   -- دالة على العمود
    WHERE email LIKE '%test%'                 -- بحث جزئي
    WHERE amount * 1.1 > 100                  -- عمليات حسابية
    ```

9. ترتيب الشروط الأمثل

    ```sql
    SELECT * FROM orders 
    WHERE customer_id = 123           -- 1. الأكثر انتقائية (فهرس)
    AND status = 'shipped'            -- 2. شرط مساواة
    AND order_date > '2023-01-01';    -- 3. نطاق زمني
    ```

    *الترتيب الأمثل:*

    1. المساواة على أعمدة مفهرسة (`customer_id`)
    2. الشروط الأخرى المساوية (`status`)
    3. النطاقات (`order_date`)

10. `snake_case` في تسمية الجداول والأعمدة

    ```sql
    -- snake_case (المعيار في PostgreSQL)
    CREATE TABLE user_orders (
        id SERIAL PRIMARY KEY,
        order_date TIMESTAMP,
        total_amount DECIMAL,
        shipping_address TEXT
    );

    -- ❌ تجنب
    CREATE TABLE UserOrders (         -- PascalCase
        OrderDate TIMESTAMP,          -- PascalCase
        totalAmount DECIMAL,          -- camelCase
    );
    ```

    *لماذا `snake_case`:*

    - مقروءة أكثر (`user_orders` vs `UserOrders`)
    - متوافقة مع `PostgreSQL`
    - المعيار في مجتمع `SQL`

11. ما هو `pg_stat_statements`؟

    ببساطة: "تقرير أداء" يخبرك بأي الاستعلامات تستهلك أكثر وقت وموارد

    ```sql
    -- تفعيله أولاً (مرة واحدة):
    CREATE EXTENSION pg_stat_statements;

    -- ثم استخدمه لمعرفة الاستعلامات البطيئة:
    SELECT 
        query, 
        total_time, 
        calls,
        mean_time
    FROM pg_stat_statements 
    ORDER BY total_time DESC 
    LIMIT 5;

    -- النتيجة ستظهر مثل:

    -- query                                   | total_time | calls | mean_time
    -- ----------------------------------------|------------|-------|-----------
    -- SELECT * FROM users WHERE email = $1    | 125.6      | 500   | 0.25
    -- UPDATE orders SET status = $1 WHERE...  | 89.3       | 200   | 0.45
    ```

    *فائدته:* يعطيك بيانات حقيقية عن أداء استعلاماتك، ليس مجرد توقعات

12. ما هو `Connection Pooling`؟

    تشبيه بسيط: مثل "موقف سيارات الأجرة" بدلاً من شراء سيارة لكل رحلة

    *بدون Connection Pooling:*

    ```python
    # ❌ سيء - اتصال جديد لكل طلب
    def handle_request():
        conn = psycopg2.connect(...)  # اتصال جديد
        # ... عمل الاستعلام
        conn.close()  # أغلق الاتصال
    ```

    *مع Connection Pooling:*

    ```python
    # ✅ ممتاز - استخدام اتصالات مجمعة
    from psycopg2 import pool

    # أنشئ مجموعة اتصالات مرة واحدة
    connection_pool = SimpleConnectionPool(
        minconn=1,
        maxconn=20,  # أقصى 20 اتصال
        host='localhost',
        database='myapp'
    )

    # استخدم من المجموعة
    def handle_request():
        conn = connection_pool.getconn()  # خذ اتصال متاح
        # ... عمل الاستعلام  
        connection_pool.putconn(conn)  # أعده للمجموعة
    ```

    *لماذا مهم؟:*

    - أسرع (تجنب فتح/إغلاق اتصالات)
    - أكثر كفاءة (إعادة استخدام الموارد)
    - يتحمل الضغط (آلاف الطلبات في الثانية)

13. ما هو `Query Optimization` عملياً؟

    **خطوات لتحسين الاستعلام:**

    *الخطوة 1: اكتشاف الاستعلامات البطيئة:*

    ```sql
    -- استخدم pg_stat_statements لاكتشاف المشاكل
    SELECT query, total_time 
    FROM pg_stat_statements 
    WHERE query LIKE '%orders%'
    ORDER BY total_time DESC;
    ```

    *الخطوة 2: تحليل خطة التنفيذ:*

    ```sql
    -- شاهد خطة التنفيذ
    EXPLAIN ANALYZE 
    SELECT * FROM orders 
    WHERE user_id = 123 AND status = 'pending';
    ```

    *الخطوة 3: التطبيقات العملية للتحسين:*

    - المشكلة: بحث بطيء على `email`

    ```sql
    -- ❌ بطيء
    SELECT * FROM users WHERE LOWER(email) = 'test@example.com';

    -- ✅ سريع (بعد إضافة الفهرس)
    CREATE INDEX idx_users_email ON users(email);
    SELECT * FROM users WHERE email = 'test@example.com';
    ```

    - المشكلة: JOIN بطيء

    ```sql
    -- ❌ غير محسن
    SELECT * FROM orders o
    JOIN users u ON o.user_id = u.id
    WHERE u.country = 'SA' AND o.total > 1000;

    -- ✅ محسن
    CREATE INDEX idx_users_country ON users(country);
    CREATE INDEX idx_orders_total ON orders(total);
    -- نفس الاستعلام لكن أسرع!
    ```

    - المشكلة: تجميع بطيء

    ```sql
    -- ❌ يمسح كل الجدول
    SELECT department, COUNT(*) 
    FROM employees 
    GROUP BY department;

    -- ✅ يستخدم الفهرس
    CREATE INDEX idx_emp_dept ON employees(department);
    -- نفس الاستعلام لكن أسرع!
    ```

    *الخطوة 4: مراقبة النتائج:*

    ```sql
    -- تحقق من التحسين
    SELECT * FROM pg_stat_statements 
    WHERE query = 'your_optimized_query';
    ```

    *الخلاصة العملية:*

    - ركز على:

        1. `EXPLAIN ANALYZE` لفهم أداء الاستعلامات
        2. الفهارس المناسبة على الأعمدة المستخدمة في `WHERE`/`JOIN`
        3. تجنب `SELECT` - اختر الأعمدة `needed` فقط
        4. `Connection Pooling` في تطبيقك

    - التحسين العملي = حل المشاكل الحقيقية التي تظهر في تطبيقك، ليس تحسين كل شيء!

14. كيفية إدراج مليون صف بكفاءة؟

    ```sql
    INSERT INTO posts (title, content, user_id)
    SELECT

    -- title
    'Post ' || generate_series(1,1000000),  -- يدمج نص "Post " مع مليون رقم (مثل "Post 1", "Post 2", ... "Post 1000000")

    -- content
    repeat('Content ', 100),  -- يكرر النص "Content " 100 مرة فتكون النتيجة: "Content Content Content ... " (تكرار 100 مرة)

    -- user_id
    (random() * 1000)::integer  --   -- يعطي أرقاما صحيحة من 0 إلى 1000 تمثل معرف المستخدمين

    FROM generate_series(1, 1000000);  -- يُنتج 1,000,000 صف، كل صف بقيمة مختلفة من السلسلة

    -- مثال بسيط (10 صفوف بدلاً من 1,000,000):

    -- | title    | content                    | user_id |
    -- |----------|----------------------------|---------|
    -- | Post 1   | Content Content Content... | 45      |
    -- | Post 2   | Content Content Content... | 78      |
    -- | ...      | ...                        | ...     |
    -- | Post 10  | Content Content Content... | 23      |
    ```

    - *الفوائد:*
        - سرعة: أسرع بكثير من إدراج صف واحد في كل مرة
        - كفاءة: استعلام واحد بدلاً من مليون استعلام
        - اختبار: مفيد جداً لإنشاء بيانات اختبار كبيرة

15. حل مشكلة التزامن (`Concurrency`)

    **المشكلة: إذا فشلت العملية في المنتصف، قد يتم خصم من حساب `A` دون إضافة إلى `B` → فقدان أموال.**

    - الحل 1: استخدام `TRANSACTIONS` (الأساسي)

    ```sql
    BEGIN;
    UPDATE accounts SET balance = balance - 100 WHERE id = 1;
    UPDATE accounts SET balance = balance + 100 WHERE id = 2;
    COMMIT;
    -- إذا حدث خطأ في أي عملية، يتم ROLLBACK تلقائياً
    ```

    - الحل 2: مع معالجة الأخطاء (`PL`/`pgSQL`)

    ```sql
    CREATE OR REPLACE FUNCTION transfer_money(
        from_account INTEGER,
        to_account INTEGER,
        amount DECIMAL
    ) RETURNS BOOLEAN AS $$
    BEGIN  -- BEGIN 1: بداية جسم الدالة (إجباري في PL/pgSQL)
        BEGIN  -- BEGIN 2: كتلة فرعية لمعالجة الأخطاء (اختياري)
            UPDATE accounts 
            SET balance = balance - amount 
            WHERE id = from_account;
            
            UPDATE accounts 
            SET balance = balance + amount 
            WHERE id = to_account;
            
            RETURN TRUE;
        EXCEPTION WHEN OTHERS THEN  -- هذه تربط بالـ BEGIN 2
            RAISE NOTICE 'خطأ في التحويل: %', SQLERRM;
            RETURN FALSE;
        END;  -- نهاية الكتلة الفرعية
    END;  -- نهاية جسم الدالة
    $$ LANGUAGE plpgsql;

    -- الاستخدام
    SELECT transfer_money(1, 2, 100);
    ```

    - الحل 3: مع التحقق من الرصيد الكافي

    ```sql
    CREATE OR REPLACE FUNCTION transfer_money(
        from_account INTEGER,
        to_account INTEGER,
        amount DECIMAL
    ) RETURNS TABLE (success BOOLEAN, message VARCHAR) AS $$
    BEGIN
        BEGIN
            -- التحقق من الرصيد أولاً
            IF (SELECT balance FROM accounts WHERE id = from_account) < amount THEN
                RETURN QUERY SELECT FALSE, 'رصيد غير كافي'::VARCHAR;
                RETURN;
            END IF;
            
            -- خصم من الحساب الأول
            UPDATE accounts 
            SET balance = balance - amount 
            WHERE id = from_account;
            
            -- إضافة للحساب الثاني
            UPDATE accounts 
            SET balance = balance + amount 
            WHERE id = to_account;
            
            RETURN QUERY SELECT TRUE, 'تم التحويل بنجاح'::VARCHAR;
            
        EXCEPTION WHEN OTHERS THEN
            RETURN QUERY SELECT FALSE, 'خطأ في التحويل'::VARCHAR;
        END;
    END;
    $$ LANGUAGE plpgsql;

    -- الاستخدام
    SELECT * FROM transfer_money(1, 2, 100);
    ```

    - الحل 4: مع `Locking` (لمنع `Race Conditions`)

    ```sql
    CREATE OR REPLACE FUNCTION transfer_money_safe(
        from_account INTEGER,
        to_account INTEGER,
        amount DECIMAL
    ) RETURNS BOOLEAN AS $$
    BEGIN
        BEGIN
            -- قفل الحسابات لمنع تعارضات متزامنة
            PERFORM * FROM accounts 
            WHERE id IN (from_account, to_account)
            ORDER BY id  -- تحسين: ترتيب ثابت لمنع Deadlocks
            FOR UPDATE;

            -- ما الفرق بين SELECT و PERFORM:
            -- الفرق الرئيسي هو أن SELECT تُستخدم لجلب البيانات وعرضها، بينما تُستخدم PERFORM لتنفيذ أوامر (مثل استدعاء دالة) في PL/pgSQL وتجاهل أي نتائج يتم إرجاعها. 
            -- SELECT: تُستخدم لاسترداد البيانات وعرضها كجزء من استعلام SQL عادي. تستخدم لعرض النتائج للمستخدم أو لتغذية بيانات استعلام آخر.
            -- PERFORM: تُستخدم في كتل PL/pgSQL عندما لا تحتاج إلى نتائج العملية. إنها طريقة لتنفيذ تعبير أو استدعاء دالة دون الاحتفاظ بالنتائج. على سبيل المثال، يمكنك استخدامها لتشغيل دالة ليس لها أي تأثير جانبي، أو لإجراء عملية تحديث ثم استخدام PERFORM لتشغيل دالة أخرى وتجاهل نتيجتها. 

            -- سياق السطر: هذا سطر داخل دالة PL/pgSQL (لذلك تُستخدم PERFORM) — يقوم بتنفيذ استعلام بدون إرجاع أي صفوف للدالة، فقط لتنفيذ تأثير جانبي (هنا: قفل الصفوف).

            -- ما يفعله بالترتيب:
            -- 1. WHERE id IN (from_account, to_account): يختار صفوف الحسابين المعنيين.
            -- 2. ORDER BY id: يؤمّن ترتيب ثابت عند الحصول على الأقفال (مثلاً الأصغر أولاً).
            -- 3. FOR UPDATE: يطلب قفل صفوف مستوى "تحديث" (row-level exclusive lock) على الصفوف المختارة.

            -- لماذا ORDER BY مهم لمنع deadlocks:
            -- لو معاملة A تقفل الحساب 1 ثم 2، ومعاملة B تقفل 2 ثم 1، قد يحصل deadlock. بفرض ترتيب موحد (مثلاً ORDER BY id) كل المعاملات تطلب الأقفال بنفس التسلسل فتختفي حالات القفل المتعارضة → يقلّ احتمال حدوث deadlock.

            -- جلب الرصيد بعد القفل (لضمان البيانات الحديثة)
            SELECT balance INTO from_balance 
            FROM accounts WHERE id = from_account;
            
            -- التحقق من الرصيد
            IF from_balance < amount THEN
                RAISE EXCEPTION 'رصيد غير كافي الرصيد المتاح: %', from_balance;
            END IF;
            
            -- العمليات الآمنة
            UPDATE accounts 
            SET balance = balance - amount 
            WHERE id = from_account;
            
            UPDATE accounts 
            SET balance = balance + amount 
            WHERE id = to_account;
            
            RETURN TRUE;
            
        EXCEPTION
        WHEN deadlock_detected THEN  -- معالجة خاصة لـ Deadlocks
            RAISE NOTICE 'تم اكتشاف deadlock - إعادة المحاولة...';
            RETURN FALSE;
        WHEN OTHERS THEN
            RAISE NOTICE 'خطأ في التحويل: %', SQLERRM;
            RETURN FALSE;
        END;
    END;
    $$ LANGUAGE plpgsql;
    ```

    - الحل 5: مع سجل المعاملات (`Audit Log`)

    ```sql
    CREATE TABLE transactions_log (
        id SERIAL PRIMARY KEY,
        from_account INTEGER,
        to_account INTEGER,
        amount DECIMAL,
        status VARCHAR,
        created_at TIMESTAMP DEFAULT now()
    );

    CREATE OR REPLACE FUNCTION transfer_money_logged(
        from_account INTEGER,
        to_account INTEGER,
        amount DECIMAL
    ) RETURNS BOOLEAN AS $$
    DECLARE
        trans_id INTEGER;
    BEGIN
        BEGIN
            -- تسجيل العملية
            INSERT INTO transactions_log (from_account, to_account, amount, status)
            VALUES (from_account, to_account, amount, 'PENDING')
            RETURNING id INTO trans_id;
            
            -- التحقق والتحويل
            IF (SELECT balance FROM accounts WHERE id = from_account) < amount THEN
                UPDATE transactions_log SET status = 'FAILED' WHERE id = trans_id;
                RETURN FALSE;
            END IF;
            
            UPDATE accounts SET balance = balance - amount WHERE id = from_account;
            UPDATE accounts SET balance = balance + amount WHERE id = to_account;
            
            -- تحديث الحالة
            UPDATE transactions_log SET status = 'SUCCESS' WHERE id = trans_id;
            RETURN TRUE;
            
        EXCEPTION WHEN OTHERS THEN
            UPDATE transactions_log SET status = 'ERROR' WHERE id = trans_id;
            RETURN FALSE;
        END;
    END;
    $$ LANGUAGE plpgsql;
    ```

    - الحل 6: حل وسيط (موصى به للتطبيقات):

    ```sql
    -- متوازن بين البساطة والأمان
    CREATE OR REPLACE FUNCTION safe_transfer(
        from_acc INTEGER,
        to_acc INTEGER, 
        amount DECIMAL
    ) RETURNS TABLE(success BOOLEAN, message TEXT) AS $$
    BEGIN
        -- التحقق الأساسي
        IF amount <= 0 THEN
            RETURN QUERY SELECT FALSE, 'المبلغ يجب أن يكون موجباً';
            RETURN;
        END IF;
        
        -- المعاملة الآمنة
        BEGIN
            UPDATE accounts SET balance = balance - amount WHERE id = from_acc;
            IF NOT FOUND THEN
                RETURN QUERY SELECT FALSE, 'الحساب المصدر غير موجود';
                RETURN;
            END IF;
            
            UPDATE accounts SET balance = balance + amount WHERE id = to_acc;
            IF NOT FOUND THEN
                -- ⭐ Rollback تلقائي إذا فشلت العملية الثانية
                RAISE EXCEPTION 'الحساب الهدف غير موجود';
            END IF;
            
            RETURN QUERY SELECT TRUE, 'تم التحويل بنجاح';
            
        EXCEPTION 
            WHEN check_violation THEN
                RETURN QUERY SELECT FALSE, 'رصيد غير كافي';
            WHEN OTHERS THEN
                RETURN QUERY SELECT FALSE, 'فشل في التحويل: ' || SQLERRM;
        END;
    END;
    $$ LANGUAGE plpgsql;
    ```

    - مثال كامل في التطبيق (مثلاً `Python`):

    ```python
    import psycopg2

    def transfer_money(from_id, to_id, amount):
        conn = psycopg2.connect("dbname=bank user=postgres")
        cur = conn.cursor()
        
        try:
            cur.execute("BEGIN;")
            
            # خصم
            cur.execute(
                "UPDATE accounts SET balance = balance - %s WHERE id = %s",
                (amount, from_id)
            )
            
            # إضافة
            cur.execute(
                "UPDATE accounts SET balance = balance + %s WHERE id = %s",
                (amount, to_id)
            )
            
            conn.commit()
            print("✅ تم التحويل بنجاح")
            return True
            
        except Exception as e:
            conn.rollback()
            print(f"❌ خطأ: {e}")
            return False
        
        finally:
            cur.close()
            conn.close()

    # الاستخدام
    transfer_money(1, 2, 100)
    ```

    - نسخة `Python` محسنة:

    ```python
    import psycopg2
    from psycopg2 import pool
    import logging

    # إعداد Connection Pool (مهم للتطبيقات الحقيقية)
    connection_pool = pool.SimpleConnectionPool(
        1, 20,  # min, max connections
        host="localhost", database="bank", 
        user="app_user", password="secure_pass"
    )

    def safe_transfer(from_id, to_id, amount, max_retries=3):
        """
        نسخة محسنة مع إعادة المحاولة لـ Deadlocks
        """
        for attempt in range(max_retries):
            conn = connection_pool.getconn()
            try:
                with conn.cursor() as cur:
                    cur.execute("BEGIN;")
                    
                    # 1. التحقق من وجود الحسابات
                    cur.execute("SELECT id FROM accounts WHERE id IN (%s, %s)", (from_id, to_id))
                    accounts = {row[0] for row in cur.fetchall()}
                    
                    if from_id not in accounts:
                        conn.rollback()
                        return False, "الحساب المصدر غير موجود"
                    if to_id not in accounts:
                        conn.rollback() 
                        return False, "الحساب الهدف غير موجود"
                    
                    # 2. التحويل
                    cur.execute(
                        "UPDATE accounts SET balance = balance - %s WHERE id = %s AND balance >= %s",
                        (amount, from_id, amount)
                    )
                    if cur.rowcount == 0:
                        conn.rollback()
                        return False, "رصيد غير كافي أو حساب غير موجود"
                    
                    cur.execute(
                        "UPDATE accounts SET balance = balance + %s WHERE id = %s",
                        (amount, to_id)
                    )
                    
                    conn.commit()
                    logging.info(f"تم التحويل بنجاح: {from_id} -> {to_id} : {amount}")
                    return True, "تم التحويل بنجاح"
                    
            except psycopg2.errors.DeadlockDetected:
                conn.rollback()
                logging.warning(f"Deadlock - المحاولة {attempt + 1}/{max_retries}")
                if attempt == max_retries - 1:
                    return False, "فشل التحويل بعد عدة محاولات"
            except Exception as e:
                conn.rollback()
                logging.error(f"خطأ في التحويل: {e}")
                return False, f"خطأ في التحويل: {e}"
            finally:
                connection_pool.putconn(conn)
        
        return False, "فشل غير متوقع"
    ```

    - *جدول مقارنة:*

    | الحل | الاستخدام الأمثل | المميزات | العيوب |
    |------|------------------|----------|--------|
    | 1. `Transactions` | تطبيقات بسيطة | 🎯 بسيط، آمن | لا يحل كل مشاكل التزامن |
    | 2. + تحقق أخطاء | تطبيقات متوسطة | 🎯 معالجة أخطاء أفضل | تعقيد متوسط |
    | 3. + تحقق رصيد | أنظمة مالية بسيطة | 🎯 يمنع الرصيد السالب | لا يمنع `Race Condition`s |
    | 4. + `Locking` | أنظمة مالية حقيقية | 🎯 آمن من التزامن | ⚠️ قد يسبب `Deadlocks` |
    | 5. + `Audit Log` | أنظمة تحتاج تتبع | 🎯 تتبع كامل | 🐌 أبطأ، تعقيد عالي |
    | 6. المتوازن | معظم التطبيقات | 🎯 أفضل توازن | - |

16. إذا كان لدي جدول `orders` به `customer_name` و `customer_phone` يتكرران في كل طلب، ما المشكلة وكيف أحلها؟

    - نستخدم  التطبيع (`Normalization`)

    ```sql
    -- ❌ تصميم سيء، كل شيء في جدول واحد (غير مطبع)
    CREATE TABLE orders (
        order_id SERIAL PRIMARY KEY,
        customer_name VARCHAR(100),      -- تكرار بيانات لكل طلب
        customer_email VARCHAR(100),     -- تكرار بيانات لكل طلب
        product_name VARCHAR(100),       -- تكرار بيانات
        product_price DECIMAL            -- قد يتغير (إذا تغير السعر، تختلط الأسعار!)!
    );
    -- المشاكل:
    -- 1. إذا غير العميل رقمه، يجب تعديل كل طلباته
    -- 2. إذا تغير سعر المنتج، تختلط الأسعار القديمة والجديدة
    -- 3. مساحة مهدرة بسبب التكرار

    -- ✅ تصميم جيد (مطبع)
    CREATE TABLE customers (
        customer_id SERIAL PRIMARY KEY,
        name VARCHAR(100),
        email VARCHAR(100)
    );

    CREATE TABLE products (
        product_id SERIAL PRIMARY KEY, 
        name VARCHAR(100),
        price DECIMAL
    );

    CREATE TABLE orders (
        order_id SERIAL PRIMARY KEY,
        customer_id INTEGER REFERENCES customers(customer_id),
        product_id INTEGER REFERENCES products(product_id),
        quantity INTEGER
    );

    ---------------------------------
    -- الأساسيات:
    ---------------------------------

    -- 1NF (First Normal Form)
    -- كل عمود يحتوي على قيمة وحيدة (لا مصفوفات، لا مجموعات)
    CREATE TABLE orders (
        order_id INT PRIMARY KEY,
        customer_id INT,      -- قيمة وحيدة
        product_id INT,       -- قيمة وحيدة  
        quantity INT,         -- قيمة وحيدة
        order_date DATE       -- قيمة وحيدة
    );
    -- ❌ لو كان product_ids = '1,2,3' هذا يخالف 1NF

    ---------------------------------

    -- 2NF (Second Normal Form)
    -- ✅ 2NF: لا توجد بيانات تعتمد على جزء من المفتاح الأساسي

    -- ❌ يخالف 2NF:
    CREATE TABLE order_items (
        order_id INT,
        product_id INT, 
        product_name VARCHAR(100),  -- يعتمد على product_id فقط (جزء من المفتاح)
        PRIMARY KEY (order_id, product_id)
    );

    -- ✅ يصبح:
    CREATE TABLE products (          -- جدول منفصل
        product_id INT PRIMARY KEY,
        product_name VARCHAR(100)
    );

    CREATE TABLE order_items (       -- الجدول الرئيسي
        order_id INT,
        product_id INT,
        PRIMARY KEY (order_id, product_id)
    );

    ---------------------------------

    -- 3NF (Third Normal Form)
    -- ✅ 3NF: لا توجد بيانات تعتمد على بيانات غير المفتاح

    -- ❌ يخالف 3NF:
    CREATE TABLE employees (
        employee_id INT PRIMARY KEY,
        name VARCHAR(100),
        department VARCHAR(100),
        department_manager VARCHAR(100)  -- يعتمد على department وليس employee_id
    );

    -- ✅ يصبح:
    CREATE TABLE departments (           -- جدول منفصل
        department_id INT PRIMARY KEY,
        name VARCHAR(100),
        manager VARCHAR(100)
    );

    CREATE TABLE employees (
        employee_id INT PRIMARY KEY,
        name VARCHAR(100),
        department_id INT REFERENCES departments(department_id)
    );
    ```

17. ماذا يحدث إذا فشلت العملية الثانية في تحويل الأموال بين حسابين؟ كيف أضمن عدم فقدان الأموال؟

    - نستخدم `ACID Properties`

    ```sql
    -- ATOMICITY (ذرية)
    BEGIN;
    UPDATE accounts SET balance = balance - 100 WHERE id = 1;
    UPDATE accounts SET balance = balance + 100 WHERE id = 2;
    COMMIT;
    -- إما تنجح كل العمليات أو تفشل كلها

    ---------------------------------

    -- CONSISTENCY (اتساق)
    -- قاعدة البيانات ترفض بيانات غير صالحة تلقائياً

    -- ✅ الاتساق يعني: البيانات دائماً صالحة

    CREATE TABLE accounts (
        id SERIAL PRIMARY KEY,
        balance DECIMAL NOT NULL CHECK (balance >= 0)  -- 👈 هذا يضمن الاتساق
    );

    -- المحرك يرفض هذا تلقائياً:
    UPDATE accounts SET balance = -100 WHERE id = 1;
    -- ❌ ERROR: check constraint violated

    -- مثال آخر:
    CREATE TABLE orders (
        id SERIAL PRIMARY KEY,
        status VARCHAR(20) CHECK (status IN ('pending', 'shipped', 'delivered'))
    );

    -- المحرك يرفض:
    UPDATE orders SET status = 'invalid_status' WHERE id = 1;
    -- ❌ ERROR: invalid value

    ---------------------------------

    -- ISOLATION (عزل)
    -- كل transaction يعمل بشكل منعزل عن الآخر

    ---------------------------------

    -- DURABILITY (متانة)  
    -- البيانات محفوظة حتى في حالة انقطاع التيار

    -- ✅ المتانة تعني: إذا قال COMMIT، البيانات محفوظة للأبد

    -- تخيل هذا السيناريو:
    BEGIN;
    UPDATE accounts SET balance = 5000 WHERE id = 1;
    COMMIT;  -- 👈 هنا البيانات أصبحت "دائمة"

    -- الآن حتى لو:
    -- ❌ انقطع الكهرباء
    -- ❌ تعطل الخادم
    -- ❌ تحطم القرص الصلب (في حدود المعقول)

    -- عند إعادة التشغيل، الرصيد سيبقى 5000
    ```

---

### The End - النهاية
