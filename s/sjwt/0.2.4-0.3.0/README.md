# Comparing `tmp/sjwt-0.2.4.tar.gz` & `tmp/sjwt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sjwt-0.2.4.tar", last modified: Mon Feb 12 13:12:12 2024, max compression
+gzip compressed data, was "sjwt-0.3.0.tar", last modified: Sun May 19 03:06:29 2024, max compression
```

## Comparing `sjwt-0.2.4.tar` & `sjwt-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2024-02-12 13:12:12.977879 sjwt-0.2.4/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      144 2024-02-12 13:12:12.977879 sjwt-0.2.4/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2024-02-12 13:12:12.977879 sjwt-0.2.4/setup.cfg
--rw-r--r--   0 andrey    (1000) andrey    (1000)      235 2024-02-12 13:12:01.000000 sjwt-0.2.4/setup.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2024-02-12 13:12:12.977879 sjwt-0.2.4/sjwt/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      194 2024-02-06 14:15:44.000000 sjwt-0.2.4/sjwt/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     7221 2024-02-12 13:11:51.000000 sjwt-0.2.4/sjwt/models.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     3019 2024-01-26 16:19:14.000000 sjwt-0.2.4/sjwt/sjwt.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2024-02-12 13:12:12.977879 sjwt-0.2.4/sjwt.egg-info/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      144 2024-02-12 13:12:12.000000 sjwt-0.2.4/sjwt.egg-info/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)      202 2024-02-12 13:12:12.000000 sjwt-0.2.4/sjwt.egg-info/SOURCES.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2024-02-12 13:12:12.000000 sjwt-0.2.4/sjwt.egg-info/dependency_links.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2024-01-26 16:19:14.000000 sjwt-0.2.4/sjwt.egg-info/not-zip-safe
--rw-r--r--   0 andrey    (1000) andrey    (1000)        5 2024-02-12 13:12:12.000000 sjwt-0.2.4/sjwt.egg-info/top_level.txt
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2024-05-19 03:06:29.653416 sjwt-0.3.0/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      144 2024-05-19 03:06:29.653416 sjwt-0.3.0/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2024-05-19 03:06:29.653416 sjwt-0.3.0/setup.cfg
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      235 2024-05-19 03:05:42.000000 sjwt-0.3.0/setup.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2024-05-19 03:06:29.649416 sjwt-0.3.0/sjwt/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      194 2024-05-19 01:52:46.000000 sjwt-0.3.0/sjwt/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     8617 2024-05-19 03:05:23.000000 sjwt-0.3.0/sjwt/models.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     3019 2024-05-19 01:52:46.000000 sjwt-0.3.0/sjwt/sjwt.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2024-05-19 03:06:29.649416 sjwt-0.3.0/sjwt.egg-info/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      144 2024-05-19 03:06:29.000000 sjwt-0.3.0/sjwt.egg-info/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      202 2024-05-19 03:06:29.000000 sjwt-0.3.0/sjwt.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2024-05-19 03:06:29.000000 sjwt-0.3.0/sjwt.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2024-05-19 01:52:46.000000 sjwt-0.3.0/sjwt.egg-info/not-zip-safe
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        5 2024-05-19 03:06:29.000000 sjwt-0.3.0/sjwt.egg-info/top_level.txt
```

### Comparing `sjwt-0.2.4/sjwt/models.py` & `sjwt-0.3.0/sjwt/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-import os
+import dotenv
 import sqlalchemy as sa
 
-from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy import Column, Integer, TIMESTAMP, ForeignKey, VARCHAR, func, Boolean, FLOAT,\
     UniqueConstraint, BigInteger
-from sqlalchemy.orm import sessionmaker
+from sqlalchemy.orm import Session, DeclarativeBase
+from src.config import settings
+dotenv.load_dotenv()
 
-Base = declarative_base()
-engine = sa.create_engine(f"postgresql+psycopg2://{os.getenv('POSTGRES_USER')}:{os.getenv('POSTGRES_PASSWORD')}@{os.getenv('POSTGRES_HOST')}:{os.getenv('POSTGRES_PORT')}/{os.getenv('POSTGRES_DB')}")
-Session = sessionmaker(bind=engine)
+# engine = sa.create_engine('sqlite:///src/bitmart_listing.db')
+engine = sa.create_engine(f"postgresql+psycopg2://{settings.POSTGRES_USER}:{settings.POSTGRES_PASSWORD}@{settings.POSTGRES_HOST}:{settings.POSTGRES_PORT}/{settings.POSTGRES_DB}")
 conn = engine.connect()
-session = Session()
+session = Session(engine)
+
+
+class Base(DeclarativeBase):
+    pass
+
 
 
 class BaseModel(Base):
     __abstract__ = True
 
     id = Column(Integer, nullable=False, unique=True, primary_key=True, autoincrement=True)
     created_at = Column(TIMESTAMP, nullable=False, default=sa.sql.func.now())
@@ -33,28 +38,28 @@
     UniqueConstraint("address", "group_id", name="adr_tgid")
 
 
 class WallepGroup(BaseModel):
     __tablename__ = 'wallet_group'
     name = Column(VARCHAR(128), nullable=True)
     telegram_id = Column(VARCHAR(128), nullable=False, index=True)
-
+    UniqueConstraint("name", "telegram_id", name="grname_tgid")
 
 class Transaction(BaseModel):
     __tablename__ = 'wallet_transaction'
-    wallet_address = Column(VARCHAR(192), nullable=False)
+    wallet_address = Column(VARCHAR(192), nullable=False, index=True)
     method_id = Column(VARCHAR(192), nullable=False)
-    timestamp = Column(TIMESTAMP, nullable=False)
+    timestamp = Column(TIMESTAMP, nullable=False, index=True)
     value = Column(FLOAT, nullable=True)
-    hash = Column(VARCHAR(256), nullable=True)
-    block_number = Column(Integer, nullable=False, unique=True)
+    hash = Column(VARCHAR(256), nullable=True, unique=True)
+    block_number = Column(Integer, nullable=False)
     block_hash = Column(VARCHAR(254), nullable=True)
     contract_address = Column(VARCHAR(196), nullable=True)
     to_adr = Column(VARCHAR(196), nullable=True)
-    from_adr = Column(VARCHAR(198), nullable=True)
+    from_adr = Column(VARCHAR(198), nullable=True, index=True)
     gas = Column(FLOAT, nullable=True)
     gasPrice = Column(FLOAT, nullable=True)
     gasUsed = Column(FLOAT, nullable=True)
     сumulativeGasUsed = Column(FLOAT, nullable=True)
     functionName = Column(VARCHAR(258), nullable=True)
 
 
@@ -102,14 +107,16 @@
     buy_count_30d = Column(FLOAT, nullable=True)
     sell_count_30d = Column(FLOAT, nullable=True)
     buy_volume_30d = Column(FLOAT, nullable=True)
     sell_volume_30d = Column(FLOAT, nullable=True)
     buy_tax = Column(VARCHAR(40), nullable=True)
     transfer_tax = Column(VARCHAR(41), nullable=True)
     sell_tax = Column(VARCHAR(42), nullable=True)
+    update_candles_1h = Column(Boolean, nullable=True, default=False)
+    update_liquidity_1h = Column(Boolean, nullable=True, default=False)
 
 
 class Candle(BaseModel):
     __tablename__ = 'candle'
 
     hash = Column(ForeignKey('coin_article.hash', ondelete='CASCADE'), index=True, nullable=False)
     received_symbol = Column(VARCHAR(60), nullable=False, index=True)
@@ -129,14 +136,40 @@
     start_block = Column(BigInteger, nullable=True)
     timestamp = Column(TIMESTAMP, nullable=False, index=True)
     volume = Column(FLOAT, nullable=True)
     exchange = Column(VARCHAR(64), nullable=True)
     UniqueConstraint("hash", "timestamp", "received_symbol", name="coin_date")
 
 
+class HourCandle(BaseModel):
+    __tablename__ = 'hour_candle'
+
+    hash = Column(ForeignKey('coin_article.hash', ondelete='CASCADE'), index=True, nullable=False)
+    received_symbol = Column(VARCHAR(60), nullable=False, index=True)
+    sell_symbol = Column(VARCHAR(60), nullable=False, index=True)
+    avg = Column(VARCHAR(36), nullable=True)
+    buy_volume = Column(FLOAT, nullable=True)
+    buys = Column(FLOAT, nullable=True)
+    close = Column(FLOAT, nullable=True)
+    end_block = Column(BigInteger, nullable=True)
+    exchange_rate = Column(FLOAT, nullable=True)
+    high = Column(FLOAT, nullable=True)
+    low = Column(FLOAT, nullable=True)
+    open = Column(FLOAT, nullable=True)
+    pair_id = Column(BigInteger, nullable=True)
+    sell_volume = Column(FLOAT, nullable=True)
+    sells = Column(FLOAT, nullable=True)
+    start_block = Column(BigInteger, nullable=True)
+    timestamp = Column(TIMESTAMP, nullable=False, index=True)
+    volume = Column(FLOAT, nullable=True)
+    exchange = Column(VARCHAR(64), nullable=True)
+    UniqueConstraint("hash", "timestamp", "received_symbol", name="coin_date")
+
+
+
 class CoinArticle(BaseModel):
     __tablename__ = 'coin_info'
 
     description = Column(VARCHAR(36), nullable=True)
     common_url = Column(VARCHAR(255), nullable=False)
     detail_url = Column(VARCHAR(255), nullable=True)
     hash = Column(ForeignKey('coin_article.hash', ondelete='CASCADE'), nullable=False, index=True)
```

### Comparing `sjwt-0.2.4/sjwt/sjwt.py` & `sjwt-0.3.0/sjwt/sjwt.py`

 * *Files identical despite different names*

