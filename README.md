<h1 align="center">Привет, я Алексей! 👋</h1>
<p align="center">
  <b>Backend Developer & Systems Engineer</b> | Go • Python • C++
  <br>
  Студент МАИ • Системное программирование • Высоконагруженные сервисы • AI-агенты и Offline RAG
</p>

<p align="center">
  <a href="https://t.me/alezovv" target="_blank"><img src="https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram" /></a>
  <a href="mailto:alezovv2523@gmail.com" target="_blank"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://github.com/Alezovv/neetcode-submissions-kd2q4x92" target="_blank"><img src="https://img.shields.io/badge/NeetCode-Blind75-00C853?style=for-the-badge&logo=leetcode&logoColor=white" alt="NeetCode" /></a>
</p>

---

### 🚀 Обо мне

* 🎓 **Образование:** Студент **МАИ** (Фундаментальная информатика и информационные технологии). Выпускник специализированных программ **VK Education** (Системное программирование на C/C++, Linux, IPC, сокеты) и **Яндекс Лицея** (Go).
* ⚙️ **Фокус:** Разработка отказоустойчивых backend-сервисов, проектирование баз данных и системного ПО, внедрение автономных и безопасных offline AI-агентов/пайплайнов.
* 💻 **Среда:** Основная ОС — **Ubuntu**. Приверженец Unix-way, строгой типизации, чистого масштабируемого кода и автоматизации рутины.
* 🧠 **Алгоритмы:** Регулярная практика структур данных и алгоритмов (Blind75, NeetCode Roadmap).

---

### 🛠️ Стек технологий

<div align="center">

| Категория | Стек и технологии |
| :--- | :--- |
| **Языки** | ![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=c%2B%2B&logoColor=white) ![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black) ![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white) |
| **Backend & Architecture** | `FastAPI` `Gin` `Django` `Clean Architecture` `gRPC` `REST API` `SQLAlchemy` |
| **Базы данных & Очереди** | `PostgreSQL` `ClickHouse` `Redis` `pgvector` `Apache Kafka` `RabbitMQ` `SQLite` |
| **Системная разработка** | `Linux IPC` `POSIX Threads` `Memory Management` `GDB` `Valgrind` `CMake / Make` |
| **AI & LLM Ops** | `Offline RAG` `pgvector` `Semantic Search` `llama.cpp (GGUF)` `ONNX Runtime` `PaddleOCR` `rubert-tiny2` |
| **DevOps & Tooling** | `Docker` `Kubernetes` `GitHub Actions` `Prometheus` `Grafana` `n8n (Self-hosted)` |

</div>

---

### 💼 Избранные проекты

#### ⚡ Systems & Low-Level

* **[Custom Relational DBMS & Storage Engine](https://github.com/Alezovv/cw_database)** *(C++14, Algorithms, File I/O)*
  * Файловая реляционная СУБД с нуля с собственным SQL-парсером (DDL/DML) и REPL-консолью.
  * Реализовал самобалансирующееся **`B*+-дерево`** для индексации полей: ускорил выборки `SELECT ... WHERE` с `O(n)` до `O(log n)` через прямое файловое смещение (offsets) без дублирования данных.
  * Внедрил механизм **String Interning** (паттерн Flyweight) для снижения оверхеда RAM при аллокациях строк.

#### 🤖 AI & High-Performance Pipelines

* **[Smart Procurement Service](https://github.com/Alezovv/RosEltorg)** *(FastAPI, PostgreSQL, pgvector, rubert-tiny2)*
  * Интеллектуальный сервис подбора тендеров под сложные номенклатуры (победный/финальный кейс хакатона **RosEltorg 2026**).
  * **Offline RAG:** Двухэтапный семантический поиск (Top-K через `pgvector` $\rightarrow$ кросс-энкодер реранжинг через `rubert-tiny2`) без внешних API. Модели вшиты в Docker-образ.
* **[DocumentRegistry](https://github.com/Alezovv/document-registry)** *(Python 3.12, ONNX, llama.cpp, SQLite, PyInstaller)*
  * Автономный offline-комбайн для обработки и семантического анализа входящих сканов/PDF.
  * Локальный пайплайн: `PyMuPDF` $\rightarrow$ `PaddleOCR` (ONNX Runtime, только при отсутствии текстового слоя) $\rightarrow$ структурированное извлечение сущностей через `llama.cpp (GGUF)`. Упакован в полностью standalone Windows-бинарник.

#### 🌐 Distributed & Backend

* **[PriceTracker API](https://github.com/Alezovv/PRICETRACKER_API)** *(FastAPI, Celery, Redis, PostgreSQL)*
  * Асинхронный сервис сбора котировок с планировщиком `Celery Beat` и кэшированием в `Redis` (TTL) для устранения оверхеда и рейт-лимитов внешних API.
* **[Contract Accounting API](https://github.com/Alezovv/contract-accounting-api)** *(FastAPI, SQLAlchemy, PostgreSQL)*
  * Сервис учета дебиторской задолженности, договоров и взаиморасчетов для малого бизнеса с валидацией транзакций.

#### 📐 Math & Computer Graphics

* **[Rigid Body Interpolation & Simulation](https://github.com/Alezovv/Python_Project)** *(Python, NumPy, SciPy, OpenGL, PyBullet)*
  * Аппроксимация и плавная интерполяция матриц трансформации твердого тела в однородных координатах + ML-регрессия для предикта промежуточных состояний.

---

### 🏆 Хакатоны и Достижения

* **🥇 RosEltorg 2026** — *Интеллектуальный поиск закупок (Offline RAG)*
  * Реализовал безопасный offline-пайплайн матчинга номенклатур на базе семантического вектора без утечки данных во внешние LLM-провайдеры.
* **✈️ Авиахакатон 2025 (МАИ / Т1)** — *Трек «Системный взлёт»*
  * Проектирование отказоустойчивой high-load архитектуры в условиях ограниченного времени.

---

### 🧩 Алгоритмическая подготовка & Статистика

<p align="center">
  <a href="https://github.com/Alezovv/neetcode-submissions-kd2q4x92">
    <img src="https://img.shields.io/badge/NeetCode-Roadmap_Progress-00C853?style=for-the-badge&logo=leetcode&logoColor=white" />
  </a>
  <img src="https://img.shields.io/badge/dynamic/json?style=for-the-badge&label=Solved&query=%24.length&url=https%3A%2F%2Fapi.github.com%2Frepos%2FAlezovv%2Fneetcode-submissions-kd2q4x92%2Fcontents%2FData%2520Structures%2520%2526%2520Algorithms&logo=leetcode&logoColor=black&color=FFA116" />
  <img src="https://img.shields.io/badge/dynamic/json?style=for-the-badge&label=Submissions&query=%24%5B0%5D.contributions&url=https%3A%2F%2Fapi.github.com%2Frepos%2FAlezovv%2Fneetcode-submissions-kd2q4x92%2Fcontributors&color=26A5E4" />
</p>

<p align="center">
  <img height="165" src="https://github-readme-stats-eight-theta.vercel.app/api?username=Alezovv&show_icons=true&theme=radical&include_all_commits=true&count_private=true" />
  <img height="165" src="https://github-readme-stats-eight-theta.vercel.app/api/top-langs/?username=Alezovv&layout=compact&theme=radical&langs_count=6" />
</p>

---

### 📫 Контакты

* **Telegram:** [@alezovv](https://t.me/alezovv)
* **Email:** [alezovv2523@gmail.com](mailto:alezovv2523@gmail.com)
* **GitHub:** [github.com/Alezovv](https://github.com/Alezovv)
* **Локация:** Москва (UTC+3)
