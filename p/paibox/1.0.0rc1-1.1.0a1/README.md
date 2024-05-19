# Comparing `tmp/paibox-1.0.0rc1.tar.gz` & `tmp/paibox-1.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paibox-1.0.0rc1.tar", max compression
+gzip compressed data, was "paibox-1.1.0a1.tar", max compression
```

## Comparing `paibox-1.0.0rc1.tar` & `paibox-1.1.0a1.tar`

### file list

```diff
@@ -1,46 +1,48 @@
--rw-r--r--   0        0        0     1218 2024-04-22 15:46:57.687398 paibox-1.0.0rc1/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2024-04-22 15:46:57.687398 paibox-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0     1005 2024-04-22 15:46:57.687398 paibox-1.0.0rc1/README.md
--rw-r--r--   0        0        0    31292 2024-04-22 15:46:57.687398 paibox-1.0.0rc1/docs/Guide-of-PAIBox.md
--rw-r--r--   0        0        0     2352 2024-04-22 15:46:57.687398 paibox-1.0.0rc1/docs/Guide-of-Test.md
--rw-r--r--   0        0        0    19453 2024-04-22 15:46:57.687398 paibox-1.0.0rc1/docs/images/Guide-基础网络搭建-全连接网络示例.png
--rw-r--r--   0        0        0     1659 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/__init__.py
--rw-r--r--   0        0        0      131 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/__init__.py
--rw-r--r--   0        0        0      394 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/checker.py
--rw-r--r--   0        0        0    13672 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/conf_template.py
--rw-r--r--   0        0        0     2079 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/constrs.py
--rw-r--r--   0        0        0     1899 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/context.py
--rw-r--r--   0        0        0    19312 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/graphs.py
--rw-r--r--   0        0        0     1044 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/graphs_types.py
--rw-r--r--   0        0        0    23915 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/mapper.py
--rw-r--r--   0        0        0    25561 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/placement.py
--rw-r--r--   0        0        0    19149 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/routing.py
--rw-r--r--   0        0        0    11780 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/segment_utils.py
--rw-r--r--   0        0        0    10082 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/base.py
--rw-r--r--   0        0        0     5192 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/collector.py
--rw-r--r--   0        0        0     1826 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/context.py
--rw-r--r--   0        0        0     1212 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/exceptions.py
--rw-r--r--   0        0        0     7015 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/mixin.py
--rw-r--r--   0        0        0     1116 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/naming.py
--rw-r--r--   0        0        0    10079 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/network.py
--rw-r--r--   0        0        0      316 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/neuron/__init__.py
--rw-r--r--   0        0        0    18461 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/neuron/base.py
--rw-r--r--   0        0        0     5469 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/neuron/neurons.py
--rw-r--r--   0        0        0      775 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/neuron/utils.py
--rw-r--r--   0        0        0      894 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/node.py
--rw-r--r--   0        0        0     5202 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/projection.py
--rw-r--r--   0        0        0      103 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/simulator/__init__.py
--rw-r--r--   0        0        0     7733 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/simulator/encoder.py
--rw-r--r--   0        0        0     1097 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/simulator/probe.py
--rw-r--r--   0        0        0     6794 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/simulator/simulator.py
--rw-r--r--   0        0        0     1571 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/simulator/utils.py
--rw-r--r--   0        0        0      531 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/synapses/__init__.py
--rw-r--r--   0        0        0    10565 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/synapses/base.py
--rw-r--r--   0        0        0    18094 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/synapses/conv_utils.py
--rw-r--r--   0        0        0     8643 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/synapses/synapses.py
--rw-r--r--   0        0        0    13881 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/synapses/transforms.py
--rw-r--r--   0        0        0      400 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/tools.py
--rw-r--r--   0        0        0     2165 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/types.py
--rw-r--r--   0        0        0     5195 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/utils.py
--rw-r--r--   0        0        0     2077 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     2371 1970-01-01 00:00:00.000000 paibox-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1371 2024-05-19 09:30:00.406718 paibox-1.1.0a1/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2024-05-19 09:30:00.406718 paibox-1.1.0a1/LICENSE
+-rw-r--r--   0        0        0      958 2024-05-19 09:30:00.406718 paibox-1.1.0a1/README.md
+-rw-r--r--   0        0        0    37145 2024-05-19 09:30:00.406718 paibox-1.1.0a1/docs/Guide-of-PAIBox.md
+-rw-r--r--   0        0        0     2816 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/__init__.py
+-rw-r--r--   0        0        0      150 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/__init__.py
+-rw-r--r--   0        0        0      394 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/checker.py
+-rw-r--r--   0        0        0    16050 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/conf_template.py
+-rw-r--r--   0        0        0     2079 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/constrs.py
+-rw-r--r--   0        0        0     3030 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/context.py
+-rw-r--r--   0        0        0    20470 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/graphs.py
+-rw-r--r--   0        0        0     1228 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/graphs_types.py
+-rw-r--r--   0        0        0    23907 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/mapper.py
+-rw-r--r--   0        0        0    25600 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/placement.py
+-rw-r--r--   0        0        0    21588 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/routing.py
+-rw-r--r--   0        0        0    12062 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/segment_utils.py
+-rw-r--r--   0        0        0    10304 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/base.py
+-rw-r--r--   0        0        0     5168 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/collector.py
+-rw-r--r--   0        0        0      143 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/components/__init__.py
+-rw-r--r--   0        0        0    30230 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/components/functional.py
+-rw-r--r--   0        0        0    12086 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/modules.py
+-rw-r--r--   0        0        0       25 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/neuron/__init__.py
+-rw-r--r--   0        0        0    18488 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/neuron/base.py
+-rw-r--r--   0        0        0     5632 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/neuron/neurons.py
+-rw-r--r--   0        0        0      775 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/neuron/utils.py
+-rw-r--r--   0        0        0     5238 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/projection.py
+-rw-r--r--   0        0        0       88 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/synapses/__init__.py
+-rw-r--r--   0        0        0    12804 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/synapses/base.py
+-rw-r--r--   0        0        0      714 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/synapses/conv_types.py
+-rw-r--r--   0        0        0    20753 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/synapses/conv_utils.py
+-rw-r--r--   0        0        0     9036 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/synapses/synapses.py
+-rw-r--r--   0        0        0    15277 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/synapses/transforms.py
+-rw-r--r--   0        0        0     1704 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/context.py
+-rw-r--r--   0        0        0     1791 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/exceptions.py
+-rw-r--r--   0        0        0     7091 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/mixin.py
+-rw-r--r--   0        0        0     1567 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/naming.py
+-rw-r--r--   0        0        0     5322 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/network.py
+-rw-r--r--   0        0        0      417 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/node.py
+-rw-r--r--   0        0        0      115 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/simulator/__init__.py
+-rw-r--r--   0        0        0     7793 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/simulator/encoder.py
+-rw-r--r--   0        0        0     1230 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/simulator/probe.py
+-rw-r--r--   0        0        0     6932 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/simulator/simulator.py
+-rw-r--r--   0        0        0     1571 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/simulator/utils.py
+-rw-r--r--   0        0        0      400 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/tools.py
+-rw-r--r--   0        0        0     2227 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/types.py
+-rw-r--r--   0        0        0     5531 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/utils.py
+-rw-r--r--   0        0        0     2241 2024-05-19 09:30:00.414718 paibox-1.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2320 1970-01-01 00:00:00.000000 paibox-1.1.0a1/PKG-INFO
```

### Comparing `paibox-1.0.0rc1/CHANGELOG.md` & `paibox-1.1.0a1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -35,7 +35,13 @@
 - 支持混合精度权重的部署
 
 ## v1.0.0rc1
 
 - 支持全展开1D/2D转置卷积算子。所有的卷积算子均支持 `padding`
 - 新增直接编码器
 - 修复后端的一些错误
+
+## v1.0.0
+
+- 提高 `paicorelib` 依赖版本至 `^1.0.0`
+- 当出现重名 `paibox.PAIBoxObject` 时将自动修改名称进行规避
+- 完善测试CI
```

### Comparing `paibox-1.0.0rc1/LICENSE` & `paibox-1.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0rc1/README.md` & `paibox-1.1.0a1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,23 @@
 
 </div>
 
 <p align="center">
     <a href="https://github.com/PAICookers/PAIBox/blob/master/pyproject.toml">
         <img src="https://img.shields.io/pypi/pyversions/paibox">
     </a>
-    <a href="https://github.com/PAICookers/PAIBox/releases/tag/v1.0.0rc1">
-        <img src="https://img.shields.io/github/v/release/PAICookers/PAIBox?include_prereleases&color=orange">
+    <a href="https://github.com/PAICookers/PAIBox/releases/tag/v1.1.0a1">
+        <img src="https://img.shields.io/github/v/release/PAICookers/PAIBox&color=orange">
     </a>
     <a href="https://www.codefactor.io/repository/github/PAICookers/PAIBox">
       <img src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIBox/master?color=red">
     </a>
     <a href="https://results.pre-commit.ci/latest/github/PAICookers/PAIBox/master">
 	   <img src="https://results.pre-commit.ci/badge/github/PAICookers/PAIBox/master.svg" alt="pre-commit.ci status">
     </a>
 </p>
 
-PAIBox使用指南：[Guide-of-PAIBox](docs/Guide-of-PAIBox.md)
+👉 用户使用指南：[Guide-of-PAIBox](docs/Guide-of-PAIBox.md)
 
 高效编写测试项目指南：[Guide-of-Test](docs/Guide-of-Test.md)
 
-TODO：[TODO List](./TODO.md)
-
 [Changelog](./CHANGELOG.md)
```

#### html2text {}

```diff
@@ -1,8 +1,7 @@
                                    # PAIBox
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_p_a_i_b_o_x_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
-    _v_/_r_e_l_e_a_s_e_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_?_i_n_c_l_u_d_e___p_r_e_r_e_l_e_a_s_e_s_&_c_o_l_o_r_=_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_f_a_c_t_o_r_/_g_r_a_d_e_/_g_i_t_h_u_b_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_/_m_a_s_t_e_r_?_c_o_l_o_r_=_r_e_d_]_[_p_r_e_-
-                               _c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]
-PAIBoxä½¿ç¨æåï¼[Guide-of-PAIBox](docs/Guide-of-PAIBox.md)
-é«æç¼åæµè¯é¡¹ç®æåï¼[Guide-of-Test](docs/Guide-of-Test.md) TODOï¼
-[TODO List](./TODO.md) [Changelog](./CHANGELOG.md)
+ _v_/_r_e_l_e_a_s_e_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_&_c_o_l_o_r_=_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_f_a_c_t_o_r_/
+    _g_r_a_d_e_/_g_i_t_h_u_b_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_/_m_a_s_t_e_r_?_c_o_l_o_r_=_r_e_d_]_[_p_r_e_-_c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]
+ð ç¨æ·ä½¿ç¨æåï¼[Guide-of-PAIBox](docs/Guide-of-PAIBox.md)
+é«æç¼åæµè¯é¡¹ç®æåï¼[Guide-of-Test](docs/Guide-of-Test.md)
+[Changelog](./CHANGELOG.md)
```

### Comparing `paibox-1.0.0rc1/docs/Guide-of-PAIBox.md` & `paibox-1.1.0a1/docs/Guide-of-PAIBox.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,30 +8,37 @@
 
 PAIBox使用 `pyproject.toml` 管理依赖。若使用Poetry：
 
 ```bash
 poetry install
 ```
 
+或者采用开发版环境
+
+```bash
+poetry install --with dev
+```
+
 若使用conda等，则手动安装如下依赖至Python虚拟环境：
 
 ```toml
 python = "^3.8"
 pydantic = "^2.0"
 numpy = "^1.24.0"
-paicorelib = "0.0.13"
+paicorelib = "^1.1.1"
+orjson = "^3.10.1" # Optional
 ```
 
 通过pip安装PAIBox：
 
 ```bash
 pip install paibox
 ```
 
-或克隆 `dev` 分支以体验开发版。
+添加 `--pre` 或克隆 `dev` 分支以使用开发版
 
 ```bash
 git clone -b dev https://github.com/PAICookers/PAIBox.git
 cd PAIBox
 ```
 
 可查看版本号以确认安装：
@@ -49,134 +56,78 @@
 
 结合**输入节点**，可以对输入数据进行脉冲编码，并传入网络中进行仿真推理。
 
 ### 神经元
 
 PAIBox提供了多种类型的神经元模型，能够实现各种特殊的功能。
 
+神经元均支持 `delay`，`tick_wait_start`，`tick_wait_end`，`keep_shape`，`unrolling_factor` 参数。
+
 ⚠️ 神经元初始膜电位为0。
 
-#### IF神经元
+#### IF
 
 IF神经元实现了经典的“积分发射”模型，其调用方式及参数如下：
 
 ```python
 import paibox as pb
 
 n1 = pb.IF(shape=10, threshold=127, reset_v=0, keep_shape=False, delay=1, tick_wait_start=1, tick_wait_end=0, name='n1')
 ```
 
 其中：
 
 - `shape`：代表神经元组的尺寸，其形式可以是整形标量、元组或列表。
 - `threshold`：神经元阈值，其形式为整数。
 - `reset_v`：神经元的重置膜电位。
+- `delay`：设定神经元输出的延迟。默认为1，即本时间步的计算结果，**下一时间步**传递至后继节点。
+- `tick_wait_start`：设定神经元启动时间。神经元将在第 `T` 个时间步时启动。0表示不启动。默认为1。
+- `tick_wait_end`：设定神经元持续工作时长。神经元将持续工作 `T` 个时间步。0表示**持续工作**。默认为0。
+- `unrolling_factor`：该参数与后端流程相关。展开因子表示神经元将被展开，部署至更多的物理核上，以降低延迟并提高吞吐率。
 - `keep_shape`：是否在仿真记录数据时保持尺寸信息，默认为 `False`。实际进行运算的尺寸仍视为一维。
-- `delay`：设定该神经元组输出的延迟。默认为1，即本时间步的计算结果，**下一时间步**传递至后继神经元。
-- `tick_wait_start`：设定该神经元组在第 `N` 个时间步时启动，0表示不启动。默认为1。
-- `tick_wait_end`：设定该神经元组持续工作 `M` 个时间步，0表示**永远持续工作**。默认为0。
-- `unrolling_factor`：该参数与后端流程相关。展开因子表示神经元将被展开，部署至更多的物理核上，以降低延迟，并提高吞吐率。
-- `name`：可选，为该对象命名。
+- `name`：神经元的名称。可选参数。
 
-#### LIF神经元
+#### LIF
 
 LIF神经元实现了“泄露-积分-发射”神经元模型，其调用方式及参数如下：
 
 ```python
 n1 = pb.LIF(shape=128, threshold=127, reset_v=0, leak_v=-1, keep_shape=False, name='n1')
 ```
 
 - `leak_v`：LIF神经元的泄露值（有符号）。其他参数含义与IF神经元相同。
 
-#### Tonic Spiking神经元
+#### Tonic Spiking
 
 Tonic Spiking神经元可以实现对持续脉冲刺激的周期性反应。
 
 ```python
 n1 = pb.TonicSpiking(shape=128, fire_step=3, keep_shape=False, name='n1')
 ```
 
 - `fire_step`：发放周期，每接收到 `N` 次刺激后发放脉冲。
 
-以下为一个简单实例：
-
-```python
-import paibox as pb
-import numpy as np
-
-n1 = pb.TonicSpiking(shape=1, fire_step=3)
-inp_data = np.ones((10,), dtype=np.bool_)
-output = np.full((10,), 0, dtype=np.bool_)
-voltage = np.full((10,), 0, dtype=np.int32)
-
-for t in range(10):
-    output[t] = n1(inp_data[t])
-    voltage[t] = n1.voltage
-
-print(output)
-
->>> [[False]
-    [False]
-    [ True]
-    [False]
-    [False]
-    [ True]
-    [False]
-    [False]
-    [ True]
-    [False]]
-```
-
-在持续的脉冲输入下，神经元进行周期性的脉冲发放。
-
-#### Phasic Spiking神经元
+#### Phasic Spiking
 
 Phasic Spiking神经元可以实现，在接受一定数量脉冲后发放，然后保持静息状态，不再发放。
 
 ```python
 n1 = pb.PhasicSpiking(shape=128, time_to_fire=3, neg_floor=10, keep_shape=False, name='n1')
 ```
 
 - `time_to_fire`：发放时间。
 - `neg_floor`：地板阈值，静息时的膜电位为其负值。
 
-以下为一个简单实例：
-
-```python
-import paibox as pb
-import numpy as np
-
-n1 = pb.PhasicSpiking(shape=1, time_to_fire=3)
-# [0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
-inp_data = np.concatenate((np.zeros((2,), np.bool_), np.ones((10,), np.bool_)))
-output = np.full((12,), 0, dtype=np.bool_)
-voltage = np.full((12,), 0, dtype=np.int32)
-
-for t in range(12):
-    output[t] = n1(inp_data[t])
-    voltage[t] = n1.voltage
+#### Always1Neuron
 
-print(output)
+Always1神经元在工作期间持续输出1。
 
->>>
-    [[False]
-    [False]
-    [False]
-    [False]
-    [ True]
-    [False]
-    [False]
-    [False]
-    [False]
-    [False]
-    [False]
-    [False]]
-```
+#### Spiking Relu
 
-当有持续性脉冲输入时，神经元会在 `time_to_step` 个时间步后发放脉冲，而后将一直保持静息状态。
+SNN模式下，具有Relu功能的神经元。当输入为1，则输出为1；输入为0，则输出为0。
 
 ### 突触
 
 #### 全连接
 
 PAIBox中，突触用于连接不同神经元组，并包含了连接关系以及权重信息。以全连接类型的突触为实例：
 
@@ -255,35 +206,37 @@
 普通的神经元连接类型，仅可以通过矩阵设置其权重 `weights`。
 
 #### 1D卷积
 
 全展开形式1D卷积为全连接突触的一种特殊表达。需**严格指定**输入神经元的尺寸与维度、卷积核权重、卷积核维度顺序与步长。对于输出神经元的具体尺寸不做严格要求。
 
 - `kernel`：卷积核权重。
-- `stride`：步长，标量。
+- `stride`：步长，标量。默认为1。
 - `padding`：填充，标量。
-- `kernel_order`：指定卷积核维度顺序为 `OIL` 或 `IOL` 排列。
+- `kernel_order`：指定卷积核维度顺序为 `OIL` 或 `IOL` 排列。默认为 `OIL`。
 - 神经元维度顺序仅支持 `CL`。
 
 ```python
 n1 = pb.IF(shape=(8, 28), threshold=1)      # Input feature map: (8, 28)
 n2 = pb.IF(shape=(16, 26), threshold=1)     # Output feature map: (16, 26)
-kernel = np.random.randint(-128, 128, size=(16, 8, 3), dtype=np.int8) # OIl
+kernel = np.random.randint(-128, 128, size=(16, 8, 3), dtype=np.int8) # OIL
 
 conv1d = pb.Conv1d(n1, n2, kernel=kernel, stride=1, padding=0, kernel_order="OIL", name="conv1d_1")
 ```
 
+⚠️ `padding` 目前不支持，默认为0。
+
 #### 2D卷积
 
 全展开形式2D卷积为全连接突触的一种特殊表达。需**严格指定**输入神经元的尺寸与维度、卷积核权重、卷积核维度顺序与步长。对于输出神经元的具体尺寸不做严格要求。
 
 - `kernel`：卷积核权重。
-- `stride`：步长，可以为标量或元组。当为标量时，对应为 `(x, x)`；当为元组时，则对应为 `(x, y)`。
+- `stride`：步长，标量或元组格式。当为标量时，对应为 `(x, x)`；当为元组时，则对应为 `(x, y)`。默认为1。
 - `padding`：填充，可以为标量或元组。当为标量时，对应为 `(x, x)`；当为元组时，则对应为 `(x, y)`。
-- `kernel_order`：指定卷积核维度顺序为 `OIHW` 或 `IOHW` 排列。
+- `kernel_order`：指定卷积核维度顺序为 `OIHW` 或 `IOHW` 排列。默认为 `OIHW`。
 - 神经元维度顺序仅支持 `CHW`。
 
 ```python
 n1 = pb.IF(shape=(8, 28, 28), threshold=1)      # Input feature map: (8, 28, 28)
 n2 = pb.IF(shape=(16, 26, 26), threshold=1)     # Output feature map: (16, 26, 26)
 kernel = np.random.randint(-128, 128, size=(16, 8, 3, 3), dtype=np.int8) # OIHW
 
@@ -302,16 +255,16 @@
 - `output_padding`：对输出特征图的一侧进行额外的填充，标量。
 - `kernel_order`：指定卷积核维度顺序为 `OIL` 或 `IOL` 排列。
 - 神经元维度顺序仅支持 `CL`。
 - 参数详细含义参见：[pytorch/ConvTranspose1d](https://pytorch.org/docs/stable/generated/torch.nn.ConvTranspose1d.html#torch.nn.ConvTranspose1d)
 
 ```python
 n1 = pb.IF(shape=(8, 28), threshold=1)      # Input feature map: (8, 28)
-n2 = pb.IF(shape=(16, 26), threshold=1)     # Output feature map: (16, 26)
-kernel = np.random.randint(-128, 128, size=(16, 8, 3), dtype=np.int8) # OIl
+n2 = pb.IF(shape=(16, 29), threshold=1)     # Output feature map: (16, 29)
+kernel = np.random.randint(-128, 128, size=(16, 8, 3), dtype=np.int8) # OIL
 
 convt1d = pb.ConvTranspose1d(n1, n2, kernel=kernel, stride=1, padding=0, output_padding=1, kernel_order="OIL", name="convt1d_1")
 ```
 
 #### 2D转置卷积
 
 全展开形式2D转置卷积为全连接突触的一种特殊表达。需**严格指定**输入神经元的尺寸与维度、卷积核权重、卷积核维度顺序与步长。对于输出神经元的具体尺寸不做严格要求。
@@ -322,25 +275,25 @@
 - `output_padding`：对输出特征图的一侧进行额外的填充，可以为标量或元组。当为标量时，对应为 `(x, x)`；当为元组时，则对应为 `(x, y)`。
 - `kernel_order`：指定卷积核维度顺序为 `OIHW` 或 `IOHW` 排列。
 - 神经元维度顺序仅支持 `CHW`。
 - 参数详细含义参见：[pytorch/ConvTranspose2d](https://pytorch.org/docs/stable/generated/torch.nn.ConvTranspose2d.html#torch.nn.ConvTranspose2d)
 
 ```python
 n1 = pb.IF(shape=(8, 28, 28), threshold=1)      # Input feature map: (8, 28, 28)
-n2 = pb.IF(shape=(16, 26, 26), threshold=1)     # Output feature map: (16, 26, 26)
+n2 = pb.IF(shape=(16, 55, 55), threshold=1)     # Output feature map: (16, 55, 55)
 kernel = np.random.randint(-128, 128, size=(16, 8, 3, 3), dtype=np.int8) # OIHW
 
 convt2d = pb.ConvTranspose2d(n1, n2, kernel=kernel, stride=2, padding=1, output_padding=0, kernel_order="OIHW", name="convt2d_1")
 ```
 
 ### 编码器
 
 PAIBox提供了有状态与无状态编码器。其中，有状态编码器是指编码过程与时间有关，将输入数据编码到一段时间窗口内。而无状态编码器是指编码过程与时间无关，每个时间步，都可以根据输入数据进行编码。
 
-⚠️ 请注意，我们只提供较为简单的编码器，以便用户在不依赖外部库的条件下实现基本编码操作；如果需要更复杂的编码，请直接使用它们。
+⚠️ 请注意，我们只提供较为简单的编码器，以便用户在不依赖外部库的条件下实现基本编码操作；如果需要更复杂的编码，请直接使用。
 
 #### 无状态编码器
 
 ##### 泊松编码
 
 泊松编码是一种常用的无状态编码。以下为一个简单实例：
 
@@ -389,15 +342,15 @@
 - `kernel_order`：指定卷积核维度顺序为 `OIHW` 或 `IOHW` 排列。
 - `tau`：膜电位时间常数。
 - `decay_input`：输入是否也会参与衰减。
 - `v_threshold`：阈值电平。
 - `v_reset`：复位电平。
 - 待编码数据维度顺序仅支持 `CHW`。
 
-其中，所使用的LIF为SpikingJelly内的 `SimpleLIFNode`。具体原理参见：[SpikingJelly/SimpleLIFNode](https://spikingjelly.readthedocs.io/zh-cn/latest/sub_module/spikingjelly.activation_based.neuron.html#spikingjelly.activation_based.neuron.SimpleLIFNode)。如果需要使用更复杂的编码，请直接使用它们。
+其中，所使用的LIF为SpikingJelly内的 `SimpleLIFNode`。具体原理参见：[SpikingJelly/SimpleLIFNode](https://spikingjelly.readthedocs.io/zh-cn/latest/sub_module/spikingjelly.activation_based.neuron.html#spikingjelly.activation_based.neuron.SimpleLIFNode)。如果需要使用更复杂的编码，请直接使用。
 
 #### 有状态编码器
 
 有状态编码器类别较多。PAIBox提供了几种有状态编码器：周期编码器 `PeriodicEncoder`、延迟编码器 `LatencyEncoder` 。
 
 ##### 周期编码器
 
@@ -530,15 +483,15 @@
 >>>
 [[3 3 3 3]
  [3 3 3 3]
  [3 3 3 3]
  [3 3 3 3]]
 ```
 
-当函数需要时间步信息，则可在函数中声明传入参数 `t` ，输入节点则在前端环境变量 `FRONTEND_ENV` 中获取时间步信息。当需要传入额外的参数时，通过 `FRONTEND_ENV.save()` 保存相关参数至前端环境变量。当函数与时间步或其他参数无关时，可使用 `**kwargs` 代替。以下为一个简单实例：
+当函数需要时间步信息，则可在函数中声明传入参数 `t` ，输入节点则在前端环境变量 `FRONTEND_ENV` 中获取时间步信息。当需要传入额外的参数时，通过 `FRONTEND_ENV.save()` 保存相关参数至前端环境变量。当函数与时间步或其他参数无关时，需使用 `**kwargs` 代替。以下为一个简单实例：
 
 ```python
 from paibox import FRONTEND_ENV
 
 def fakeout_with_t(t, bias, **kwargs): # ignore other arguments except `t` & `bias`
     return np.ones((4, 4)) * t + bias
 
@@ -592,25 +545,145 @@
 >>>
     [[ True False  True  True]
     [ True False  True  True]
     [False  True  True  True]
     [ True  True  True False]]
 ```
 
-### 网络模型
+## 功能模块
+
+多个基础组件可以组成具有特定功能的模块(module)。在实例化与仿真中，它们作为一个整体，而在后端中则会被拆解，并由多个基础组件构建。不同于基本的神经网络组件——神经元与突触的常规使用模式：
+
+- 在实例化时，其运作机制借鉴了“突触”的连接特性，要求在初始化阶段指定与其相连的前级神经元作为输入源，这些神经元的输出信号将作为进行逻辑运算的操作数。
+- 该模块完成运算后的输出效果，则表现为一个具有独立输出能力的“神经元”，其输出接口的设计完全符合神经元的标准形式。这意味着其输出脉冲可作为后继突触的输入。
+- 后端构建时，模块将拆分成一或多个神经元节点与突触。所构建的基础组件尺寸由模块连接的操作数尺寸决定。
+
+功能模块均支持 `delay`，`tick_wait_start`，`tick_wait_end`，`keep_shape` 参数。
+
+### 逻辑运算
+
+逻辑运算模块实现了 `numpy` 中的位逻辑运算操作（例如 `&` 与 `numpy.bitwise_and` 等），可对接收到的一或多个输出脉冲进行逻辑运算，并产生脉冲输出。PAIBox提供了逻辑与、或、非、异或：`BitwiseAND`，`BitwiseOR`，`BitwiseNOT`，`BitwiseXOR`。以位与为例：
+
+```python
+import paibox as pb
+
+class Net(pb.DynSysGroup):
+    def __init__(self):
+        super().__init__()
+        self.n1 = pb.IF((10,), 1, 0, delay=1, tick_wait_start=1)
+        self.n2 = pb.IF((10,), 1, 0, delay=1, tick_wait_start=1)
+        self.and1 = pb.BitwiseAND(self.n1, self.n2, delay=1, tick_wait_start=2)
+        self.n3 = pb.IF((10,), 1, 0, delay=1, tick_wait_start=self.and1.tick_wait_start + self.and1.external_delay + 1)
+        self.s3 = pb.FullConn(self.and1, self.n3, conn_type=pb.SynConnType.All2All)
+```
+
+其中：
+
+- `neuron_a`：第一个操作数。
+- `neuron_b`：第二个操作数。
+- `delay`：设定模块输出的延迟。默认为1，即本时间步的计算结果，**下一时间步**传递至后继节点。
+- `tick_wait_start`：设定模块启动时间。模块将在第 `T` 个时间步时启动。0表示不启动。默认为1。
+- `tick_wait_end`：设定模块持续工作时长。模块将持续工作 `T` 个时间步。0表示**持续工作**。默认为0。
+- `keep_shape`：是否在仿真记录数据时保持尺寸信息，默认为 `False`。实际进行运算的尺寸仍视为一维。
+- `name`：模块的名称。可选参数。
+
+⚠️ 模块的属性 `external_delay` 用于表示其相对于外部的内部固有延迟。这是由具体的后端构建形式决定的，不可更改。上述示例中，位与计算结果将输出至 `n3` 中。默认情况下，`n3` 将在位与计算结果输出后启动，因此其启动时间为 `and1` 的启动时间+固有延迟+1。
+
+### 延迟链
 
-在PAIBox中，可以通过继承 `DynSysGroup`（或 `Network`）来实现，并在其中例化神经元与突触组件，完成网络模型的构建。以一个简单的两层全连接网络为例：
+用于实现神经元延迟输出。使用方式如下：
+
+```python
+n1 = pb.IF((10,), 1, 0, delay=1, tick_wait_start=1)
+n1_delay_out = pb.DelayChain(n1, chain_level=5, delay=1, tick_wait_start=2)
+n2 = pb.SpikingRelu((10,), delay=1, tick_wait_start=n1_delay_out.tick_wait_start + n1_delay_out.external_delay)
+```
+
+其中：
+
+- `neuron`：进行延迟输出的神经元。
+- `chain_level`：延迟链的级数，即延迟的时间步。注意，这与 `delay` 含义不同：延迟链内部会建立多级神经元（类似buffer），以实现数据的延迟传递，而 `delay` 会使得神经元输出寄存的位置延后，后继节点的启动时间需要提前，这将导致其在前级**有效输出**前就进行了计算。
+
+### 平均/最大池化
+
+目前仅提供2D池化：`SpikingAvgPool2d`、`SpikingMaxPool2d`。以平均池化为例：
+
+```python
+ksize = (3, 3)
+stride = None # default is ksize
+n1 = pb.SpikingRelu(shape, tick_wait_start=1)
+pool2d = pb.SpikingAvgPool2d(n1, ksize, None, tick_wait_start=2)
+n2 = pb.SpikingRelu(pool2d.shape_out, delay=1, tick_wait_start=3)
+s3 = pb.FullConn(pool2d, n2, conn_type=pb.SynConnType.One2One)
+```
+
+其中：
+
+- `neuron`：待池化的神经元。
+- `kernel_size`：池化窗口的尺寸，标量或元组格式。当为标量时，对应为 `(x, x)`；当为元组时，则对应为 `(x, y)`。
+- `stride`：步长，可选参数，标量或元组格式，默认为 `None`，即池化窗口的尺寸。
+- 神经元维度顺序仅支持 `CHW`。
+
+### 脉冲加、减
+
+脉冲加减法与数的加减法存在差异。对脉冲进行加减，运算结果将在较长时间步上体现。例如，在 `T=1` 时刻两神经元均输出1，则将在 `T=2,3` 时刻产生输出脉冲。以下为脉冲加减法运算示例。其中，输入为 `T=12` 脉冲序列，输出为 `T=20` 脉冲序列。
+
+```python
+inpa = np.array([1, 0, 0, 1, 0, 0, 0, 0, 1, 1, 1, 1], np.bool_)
+inpb = np.array([0, 0, 1, 1, 0, 0, 0, 1, 0, 0, 1, 0], np.bool_)
+
+# 脉冲加结果
+>>> np.array([0, 1, 0, 1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0], np.bool_)
+# 脉冲减结果
+>>> np.array([0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0], np.bool_)
+```
+
+`SpikingAdd`，`SpikingSub` 的使用方式与逻辑运算模块相同：
+
+```python
+n1 = pb.IF((10,), 1, 0, delay=1, tick_wait_start=1)
+n2 = pb.IF((10,), 1, 0, delay=1, tick_wait_start=1)
+add1 = pb.SpikingAdd(n1, n2, overflow_strict=False, delay=1, tick_wait_start=2) # n1 + n2
+sub1 = pb.SpikingSub(n1, n2, overflow_strict=False, delay=1, tick_wait_start=2) # n1 - n2
+```
+
+其中：
+
+- `neuron_a`：第一个操作数。
+- `neuron_b`：第二个操作数。在减法中作被减数。
+- `overflow_strict`：是否严格检查运算结果溢出。如果启用，则在仿真中，当脉冲加、减运算结果溢出时将报错。默认为 `False`。
+
+### 转置
+
+PAIBox提供了转置模块 `Transpose2d`，`Transpose3d`，用于实现二维、三维矩阵的转置。对于转置，需要**指定**输入神经元的尺寸、转置顺序（仅三维转置需要）。使用方法与逻辑运算模块相同：
+
+```python
+n1 = pb.IF((32, 16), 1, 0, delay=1, tick_wait_start=1)
+t2d = pb.Transpose2d(n1, tick_wait_start=2)
+
+n2 = pb.IF((32, 16, 24), 1, 0, delay=1, tick_wait_start=1)
+t3d = pb.Transpose3d(n2, axes=(1, 2, 0), tick_wait_start=2)
+```
+
+其中：
+
+- `neuron`：待转置其输出脉冲的神经元。对于二维转置，支持输入尺寸为1或2维；对于三维转置，支持输入尺寸为2或3维。尺寸不足时，自动补1。
+- `axes`：（仅三维转置）如果指定，则必须是包含 `[0,1,…,N-1]` 排列的元组或列表，其中 `N` 是矩阵的轴（维度）数。返回数组的第 `i` 轴将对应于输入的编号为 `axes[i]` 的轴。若未指定，则默认为 `range(N)[::-1]`，这将反转轴的顺序。具体参数含义参见：[numpy.transpose](https://numpy.org/doc/1.26/reference/generated/numpy.transpose.html#numpy.transpose)
+
+## 网络模型
+
+在PAIBox中，可以通过继承 `DynSysGroup`（或 `Network`）来实现，并在其中例化基础组件与功能模块，完成网络模型的构建。以一个简单的两层全连接网络为例：
 
 <p align="center">
     <img src="images/Guide-基础网络搭建-全连接网络示例.png" alt="基础网络搭建-全连接网络示例" style="zoom:50%">
 </p>
 
-#### 定义网络模型
+### 网络构建
 
-要搭建上述网络，首先继承 `pb.Network` 并在子类 `fcnet` 中初始化网络。先例化输入节点 `i1` 与两个神经元组 `n1`、 `n2`，然后例化两个突触 `s1`、 `s2` ，将三者连接起来。其中，输入节点为泊松编码器。
+要构建上述网络，首先继承 `pb.Network` 并在子类 `fcnet` 中初始化网络。先例化输入节点 `i1` 与两个神经元组 `n1`、 `n2`，然后例化两个突触 `s1`、 `s2` ，将三者连接起来。其中，输入节点为泊松编码器。
 
 ```python
 import paibox as pb
 
 class fcnet(pb.Network):
     def __init__(self, weight1, weight2):
         super().__init__()
@@ -619,15 +692,15 @@
         self.i1 = pb.InputProj(input=pe, shape_out=(784,))
         self.n1 = pb.IF(128, threshold=128, reset_v=0, tick_wait_start=1)
         self.n2 = pb.IF(10, threshold=128, reset_v=0, tick_wait_start=2)
         self.fc1 = pb.FullConn(self.i1, self.n1, weights=weight1, conn_type=pb.SynConnType.All2All)
         self.fc2 = pb.FullConn(self.n1, self.n2, weights=weight2, conn_type=pb.SynConnType.All2All)
 ```
 
-#### 容器类型
+### 容器类型
 
 PAIBox提供 `NodeList`、`NodeDict` 容器类型，可批量化操作网络基本组件。例如，
 
 ```python
 import paibox as pb
 l1 = pb.NodeList()
 
@@ -636,58 +709,56 @@
 
 for i in range(5):
     l1.append(pb.LIF(10, threshold=5, reset_v=0))
 ```
 
 如此，我们共例化了10个神经元，包括5个IF神经元、5个LIF神经元。在容器内的基本组件可通过下标进行访问、与其他基本组件连接。这与一般容器类型的用法相同。
 
-#### 嵌套网络
+### 嵌套网络
 
 有时网络中会重复出现类似的结构，这时先构建子网络，再多次例化复用是个不错的选择。
 
 ```python
-froom typing import Optional
+from typing import Optional
 import paibox as pb
 
 class ReusedStructure(pb.Network):
     def __init__(self, weight, tws, name: Optional[str] = None):
         super().__init__(name=name)
 
         self.pre_n = pb.LIF((10,), 10, tick_wait_start=tws)
         self.post_n = pb.LIF((10,), 10, tick_wait_start=tws+1)
         self.fc = pb.FullConn(
             self.pre_n, self.post_n, conn_type=pb.SynConnType.All2All, weights=weight
         )
 
 class Net(pb.Network):
     def __init__(self, w1, w2):
+        super().__init__()
+
         self.inp1 = pb.InputProj(1, shape_out=(10,))
-        subnet1 = ReusedStructure(w1, tws=1, name="Reused_Struct_0")
-        subnet2 = ReusedStructure(w2, tws=3, name="Reused_Struct_1")
+        self.subnet1 = ReusedStructure(w1, tws=1, name="Reused_Struct_0")
+        self.subnet2 = ReusedStructure(w2, tws=3, name="Reused_Struct_1")
         self.fc1 = pb.FullConn(
             self.inp1,
-            subnet1.pre_n,
+            self.subnet1.pre_n,
             conn_type=pb.SynConnType.One2One,
         )
         self.fc2 = pb.FullConn(
-            subnet1.post_n,
-            subnet2.pre_n,
+            self.subnet1.post_n,
+            self.subnet2.pre_n,
             conn_type=pb.SynConnType.One2One,
         )
 
-        super().__init__(subnet1, subnet2) # Necessary!
-
 w1 = ...
 w2 = ...
 net = Net(w1, w2)
 ```
 
-上述示例代码中，我们先创建需复用的子网络 `ReusedStructure`，其结构为 `pre_n` -> `fc` -> `post_n`。而后，在父网络 `Net` 中实例化两个子网络 `subnet1`、 `subnet2`，并与父网络其他部分连接，此时网络结构为：`inp1` -> `fc1` -> `subnet1` -> `fc22` -> `subnet2`。最后，在为 `pb.Network` 初始化时，传入子网络 `subnet1`、 `subnet2`。由此，父网络 `Net` 才能发现子网络组件。如果想取到 `Net` 内的 `subnet1` 对象，可通过索引其名字 `Net["Reused_Struct_0"]` 取到。
-
-上述示例为一个二级嵌套网络，对于三级嵌套网络或更高（不推荐使用），可参考上述方式构建。
+上述示例代码中，我们先创建需复用的子网络 `ReusedStructure`，其结构为 `pre_n` -> `fc` -> `post_n`。而后，在父网络 `Net` 中实例化两个子网络 `subnet1`、 `subnet2`，并与父网络其他部分连接，此时网络结构为：`inp1` -> `fc1` -> `subnet1` -> `fc22` -> `subnet2`。上述示例为一个二级嵌套网络，对于三级或更高级嵌套网络，可参考上述方式构建。
 
 ## 仿真
 
 ### 仿真器
 
 例化网络后，即可构建仿真器：
 
@@ -706,15 +777,14 @@
 ### 探针
 
 在仿真过程中，用户需要检测某一层神经元的膜电位或输出、突触的输出等信息，这可通过**探针**实现。探针告知仿真器在仿真时需要记录哪些信息。使用探针的方式有如下两种：
 
 1. 在构建网络时，直接设置探针，即在网络内部例化探针对象。
 2. 在外部例化探针，并调用 `add_probe` 将其添加至仿真器内。仿真器内部将保存所有探针对象。
 3. 调用 `remove_probe` 方法可移除探针及其仿真数据。
-4. 请注意，目前探针仅能在最外层父网络内例化，子网络内的探针无法被发现。
 
 例化探针时需指定：
 
 - `target`: 监测对象，必须是 `DynamicSys` 类。
 - `attr`：监测的属性，如 `spike`、`output` 等，字符串类型，这将监测属性 `target.attr`。
 
 基于上述仿真示例，我们添加几个探针：
@@ -775,15 +845,18 @@
 
 例化 `Mapper`，传入所构建的网络模型，进行编译，最后导出帧即可。
 
 ```python
 mapper = pb.Mapper()
 mapper.build(fcnet)
 graph_info = mapper.compile(weight_bit_optimization=True, grouping_optim_target="both")
-mapper.export(write_to_file=True, fp="./debug/", format="bin", split_by_coordinate=False, local_chip_addr=(0, 0), export_core_params=False)
+mapper.export(write_to_file=True, fp="./debug/", format="bin", split_by_coord=False, export_core_params=False)
+
+graph_info.n_core_required
+>>> 999
 
 # Clear all the results
 mapper.clear()
 ```
 
 其中，编译时有如下参数可指定：
 
@@ -792,40 +865,42 @@
 - 同时，该方法将返回字典形式的编译后网络的信息。
 
 导出时有如下参数可指定：
 
 - `write_to_file`: 是否将配置帧导出为文件。默认为 `True`。
 - `fp`：导出目录。若未指定，则默认为后端配置选项 `build_directory` 所设置的目录（当前工作目录）。
 - `format`：导出交换文件格式，可以为 `bin`、`npy` 或 `txt`。默认为 `bin`。
-- `split_by_coordinate`：是否将配置帧以每个核坐标进行分割，由此生成的配置帧文件命名为"config_core1"、"config_core2"等。默认为 `False`，即最终导出为一个文件。
-- `local_chip_addr`：本地芯片坐标，元组格式表示。默认为后端配置项 `local_chip_addr` 所设置的默认值。
+- `split_by_coord`：是否将配置帧以每个核坐标进行分割，由此生成的配置帧文件命名形如"config_core1"、"config_core2"。默认为 `False`，即最终导出为一个文件。
 - `export_core_params`: 是否导出实际使用核参数至json文件，以直观显示实际使用核的配置信息。默认为 `False`。
 
 同时，该方法将返回模型的配置项字典 `GraphInfo`，包括：
 
 - `input`：输入节点信息字典。
 - `output`：输出目的地信息字典。
 - `memebers`：中间层所在物理核的配置项字典。
-- `inherent_timestep`：网络模型的最长时间步。
-- `n_core_required`：网络模型需要的物理核数目。
+- `inherent_timestep`：网络的最长时间步。
+- `n_core_required`：网络**需要**的物理核数目。
+- `n_core_occupied`：网络**实际占用**的物理核数目。
 - `extras`：其他额外的网络信息字典，例如，编译后的网络名称。
 
 ### 后端配置项
 
-与后端相关的配置项由 `BACKEND_CONFIG` 统一保存与访问，例如上述**编译选项**、`build_directory`、`local_chip_addr` 等。如下所示，对常用的配置项进行读取与修改：
+与后端相关的配置项由 `BACKEND_CONFIG` 统一保存与访问，例如上述**编译选项**、`build_directory`、`target_chip_addr` 等。如下所示，对常用的配置项进行读取与修改：
 
-1. 本地芯片地址 `local_chip_addr`
+1. 本地芯片地址 `target_chip_addr`，支持**多芯片配置**。
 
    ```python
    # Read
-   BACKEND_CONFIG.local_chip_addr
-   >>> Coord(0, 0)
+   BACKEND_CONFIG.target_chip_addr
+   >>> [Coord(0, 0)]
 
-   # Modify
-   BACKEND_CONFIG.local_chip_addr = (1, 1)
+   # Single chip
+   BACKEND_CONFIG.target_chip_addr = (1, 1)
+   # Multiple chips
+   BACKEND_CONFIG.target_chip_addr = [(0, 0), (0, 1), (1, 0)]
    ```
 
 2. 输出芯片地址（测试芯片地址） `output_chip_addr`
 
    ```python
    # Read
    BACKEND_CONFIG.output_chip_addr
@@ -835,14 +910,16 @@
 
    # Modify
    BACKEND_CONFIG.output_chip_addr = (2, 0)
    # or
    BACKEND_CONFIG.test_chip_addr = (2, 0)
    ```
 
+   ⚠️ 请确保输出芯片地址不与本地芯片地址重叠。
+
 3. 编译后配置信息等文件输出目录路径 `output_dir`，默认为用户当前工作目录
 
    ```python
    # Read
    BACKEND_CONFIG.output_dir
    >>> Path.cwd() # Default is your current working directory
```

### Comparing `paibox-1.0.0rc1/paibox/backend/conf_template.py` & `paibox-1.1.0a1/paibox/backend/conf_template.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import json
-from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
 from typing import Any, ClassVar, Dict, List, Literal, NamedTuple, TypedDict
 
 import numpy as np
 from numpy.typing import NDArray
 from paicorelib import (
     LCN_EX,
     AxonCoord,
+    ChipCoord,
     Coord,
+    CoordAddr,
     HwConfig,
     InputWidthFormat,
     MaxPoolingEnable,
     NeuronAttrs,
     NeuronDestInfo,
     ParamsReg,
 )
@@ -27,16 +27,49 @@
 from paicorelib.framelib import types
 from paicorelib.framelib.frame_gen import OfflineFrameGen
 from paicorelib.framelib.utils import np2bin, np2npy, np2txt
 from typing_extensions import NotRequired, TypeAlias
 
 from paibox.base import NeuDyn
 
+from .context import _BACKEND_CONTEXT
 from .graphs_types import NodeName
 
+try:
+    import orjson  # type: ignore
+
+    _use_orjson = True
+
+    def PAIConfigJsonDefault(o: Any):
+        if isinstance(o, Coord):
+            return o.address
+        elif isinstance(o, NeuronDestInfo):
+            return o.model_dump(by_alias=True)
+
+        raise TypeError
+
+except ModuleNotFoundError:
+    import json
+
+    _use_orjson = False
+
+    class PAIConfigJsonEncoder(json.JSONEncoder):
+        def default(self, o: Any) -> Any:
+            if isinstance(o, Coord):
+                return o.address
+            elif isinstance(o, Enum):
+                return o.value
+            elif isinstance(o, np.ndarray):
+                return o.tolist()
+            elif isinstance(o, NeuronDestInfo):
+                return o.model_dump(by_alias=True)
+            else:
+                return super().default(o)
+
+
 # Prevent import errors caused by changes in type definitions in paicorelib.
 if hasattr(types, "FRAME_DTYPE"):
     FRAME_DTYPE = types.FRAME_DTYPE
 else:
     FRAME_DTYPE = np.uint64
 
 if hasattr(types, "FrameArrayType"):
@@ -98,16 +131,15 @@
         dest_info = NeuronDestInfo.model_validate(self._asdict(), strict=True)
         dict_ = dest_info.model_dump(by_alias=True)
 
         return dict_
 
     def __json__(self) -> Dict[str, Any]:
         """Dump the configs into json for debugging."""
-        dest_info = NeuronDestInfo.model_validate(self._asdict(), strict=True)
-        dict_ = dest_info.model_dump(by_alias=True)
+        dict_ = self.export()
 
         for var in self._extra_params:
             dict_[var] = getattr(self, var)
 
         return dict_
 
 
@@ -125,16 +157,15 @@
 
 class ConfigTemplate:
     """A configuration template."""
 
     pass
 
 
-@dataclass(eq=False)
-class NeuronConfig(ConfigTemplate):
+class NeuronConfig(NamedTuple):
     _extra_params = (
         "n_neuron",
         "addr_ram",
         "addr_offset",
     )
     """Extra parameters for debugging."""
 
@@ -189,33 +220,34 @@
             n_neuron,
             addr_ram,
             addr_offset,
             attrs,
             neuron_dest_info,
         )
 
-    def __json__(self) -> Dict[str, Any]:
-        """Dump the configs into json for debugging."""
+    def export(self) -> Dict[str, Any]:
         dict_ = self.neuron_attrs.model_dump(
             by_alias=True,
             # exclude={"dest_info": self.params_ram.dest_info._exclude_vars},
         )
+        dict_.update(self.neuron_dest_info.model_dump(by_alias=True))
 
-        dict_.update(
-            self.neuron_dest_info.model_dump(by_alias=True)
-        )  # compatible for py3.8
+        return dict_
+
+    def __json__(self) -> Dict[str, Any]:
+        """Dump the configs into json for debugging."""
+        dict_ = self.export()
 
         for var in self._extra_params:
             dict_[var] = getattr(self, var)
 
         return dict_
 
 
-@dataclass(eq=False)
-class CorePlacementConfig(ConfigTemplate):
+class CorePlmConfig(NamedTuple):
     _extra_params = ()
     """Extra parameters for debugging."""
 
     random_seed: int
     weight_ram: NDArray[np.uint64]
     params_reg: ParamsReg
     neuron_configs: Dict[NeuDyn, NeuronConfig]
@@ -231,183 +263,183 @@
         return cls(
             random_seed,
             weight_ram,
             ParamsReg.model_validate(core_config._asdict(), strict=True),
             neuron_configs,
         )
 
-    def __json__(self) -> Dict[str, Any]:
-        """Dump the configs into json for debugging."""
+    def export(self) -> Dict[str, Any]:
         dict_ = {
             "name": self.params_reg.name,
             "random_seed": self.random_seed,
             "neuron_rams": dict(),
             **self.params_reg.model_dump(by_alias=True),
         }
 
         for neu, neu_config in self.neuron_configs.items():
-            dict_["neuron_rams"][neu.name] = neu_config.__json__()
+            dict_["neuron_rams"][neu.name] = neu_config.export()
+
+        return dict_
+
+    def __json__(self) -> Dict[str, Any]:
+        """Dump the configs into json for debugging."""
+        dict_ = self.export()
 
         for var in self._extra_params:
             dict_[var] = getattr(self, var)
 
         return dict_
 
 
-class EmptyCorePlacementConfig(CorePlacementConfig):
+class EmptyCorePlmConfig(CorePlmConfig):
     _default_seed: ClassVar[int] = 0
     _default_zero_wram: ClassVar[NDArray[np.uint64]] = np.zeros(
         (HwConfig.ADDR_RAM_MAX, 18), dtype=np.uint64
     )
+    _default_neuron_conf = {}  # don't care
 
     @classmethod
     def encapsulate(cls, core_config: CoreConfig):
         return cls(
             cls._default_seed,
             cls._default_zero_wram,
             ParamsReg.model_validate(core_config._asdict(), strict=True),
-            {},
+            cls._default_neuron_conf,
         )
 
 
-InputNodeInfo: TypeAlias = Dict[NodeName, NeuronDest]
-OutputDestInfo: TypeAlias = Dict[NodeName, Dict[int, NeuronDestInfo]]
-CorePlacementInfo: TypeAlias = Dict[Coord, CorePlacementConfig]
+InputNodeConf: TypeAlias = Dict[NodeName, NeuronDest]
+OutputDestConf: TypeAlias = Dict[NodeName, Dict[CoordAddr, NeuronDestInfo]]
+CorePlmConfInChip: TypeAlias = Dict[Coord, CorePlmConfig]
+CorePlmConf: TypeAlias = Dict[ChipCoord, CorePlmConfInChip]
 
 
 class GraphInfo(TypedDict):
     """Information of compiled graph.
 
     TODO Optimize the data structure
     """
 
-    input: InputNodeInfo
-    output: OutputDestInfo
-    members: CorePlacementInfo
+    input: InputNodeConf
+    output: OutputDestConf
+    members: CorePlmConf
     inherent_timestep: int
     n_core_required: int
     """The actual used cores."""
     n_core_occupied: int
     """The occupied cores, including used & wasted."""
     extras: NotRequired[Dict[str, Any]]
 
 
 def gen_config_frames_by_coreconf(
-    config_dict: Dict[Coord, CorePlacementConfig],
-    target_chip_coord: Coord,
+    config_dict: CorePlmConf,
     write_to_file: bool,
     fp: Path,
     split_by_coord: bool,
     format: Literal["txt", "bin", "npy"],
 ) -> Dict[Coord, FrameArrayType]:
-    """Generate configuration frames by given the `CorePlacementConfig`.
+    """Generate configuration frames by given the `CorePlmConfig`.
 
     Args:
         - config_dict: the dictionary of configurations.
-        - target_chip_coord: local chip coordinate.
         - write_to_file: whether to write frames to file.
         - fp: If `write_to_file` is `True`, specify the path.
         - split_by_coord: whether to split the generated frames file by the core coordinates.
         - format: `txt`, `bin`, or `npy`.
     """
 
     def _write_to_f(name: str, array: FrameArrayType) -> None:
-        nonlocal fp, format
-
         _fp = fp / (name + f".{format}")
         if format == "npy":
             np2npy(_fp, array)
         elif format == "bin":
             np2bin(_fp, array)
         else:
             np2txt(_fp, array)
 
     _default_rid = RId(0, 0)
     _debug_dict: Dict[Coord, Dict[str, Any]] = dict()
     frame_arrays_on_core: Dict[Coord, FrameArrayType] = dict()
 
-    for core_coord, v in config_dict.items():
-        # 1. Only one config frame type I for each physical core.
-        config_frame_type1 = OfflineFrameGen.gen_config_frame1(
-            target_chip_coord,
-            core_coord,
-            _default_rid,
-            v.random_seed,
-        )
-
-        # 2. Only one config frame type II for each physical core.
-        config_frame_type2 = OfflineFrameGen.gen_config_frame2(
-            target_chip_coord,
-            core_coord,
-            _default_rid,
-            v.params_reg,
-        )
-
-        # 3. Iterate all the neuron segments inside the physical core.
-        config_frame_type3 = []
-        for neu_conf in v.neuron_configs.values():
-            config_frame_type3.append(
-                OfflineFrameGen.gen_config_frame3(
-                    target_chip_coord,
-                    core_coord,
-                    _default_rid,
-                    neu_conf.addr_offset,
-                    neu_conf.n_neuron,
-                    neu_conf.neuron_attrs,
-                    neu_conf.neuron_dest_info,
-                    lcn_ex=v.params_reg.lcn_extension,
-                    weight_precision=v.params_reg.weight_precision,
-                )
+    for chip_coord, conf_in_chip in config_dict.items():
+        for core_coord, v in conf_in_chip.items():
+            # 1. Only one config frame type I for each physical core.
+            config_frame_type1 = OfflineFrameGen.gen_config_frame1(
+                chip_coord, core_coord, _default_rid, v.random_seed
             )
 
-        if config_frame_type3:
-            frame3 = np.concatenate(
-                [f.value for f in config_frame_type3], dtype=FRAME_DTYPE, casting="no"
+            # 2. Only one config frame type II for each physical core.
+            config_frame_type2 = OfflineFrameGen.gen_config_frame2(
+                chip_coord, core_coord, _default_rid, v.params_reg
             )
-        else:
-            frame3 = np.asarray([], dtype=FRAME_DTYPE)
 
-        # 4. Only one config frame type IV for each physical core.
-        n_addr_write = v.params_reg.num_dendrite  # The number of address to write
-        if n_addr_write > 0:
-            config_frame_type4 = OfflineFrameGen.gen_config_frame4(
-                target_chip_coord,
-                core_coord,
-                _default_rid,
-                0,
-                18 * n_addr_write,
-                v.weight_ram[:n_addr_write],
-            )
-        else:
-            config_frame_type4 = None
+            # 3. Iterate all the neuron segments inside the physical core.
+            config_frame_type3 = []
+            for neu_conf in v.neuron_configs.values():
+                config_frame_type3.append(
+                    OfflineFrameGen.gen_config_frame3(
+                        chip_coord,
+                        core_coord,
+                        _default_rid,
+                        neu_conf.addr_offset,
+                        neu_conf.n_neuron,
+                        neu_conf.neuron_attrs,
+                        neu_conf.neuron_dest_info,
+                        lcn_ex=v.params_reg.lcn_extension,
+                        weight_precision=v.params_reg.weight_precision,
+                    )
+                )
 
-        _debug_dict[core_coord] = {
-            "config1": config_frame_type1,
-            "config2": config_frame_type2,
-            "config3": config_frame_type3,
-            "config4": config_frame_type4,
-        }
+            if config_frame_type3:
+                frame3 = np.concatenate(
+                    [f.value for f in config_frame_type3],
+                    dtype=FRAME_DTYPE,
+                    casting="no",
+                )
+            else:
+                frame3 = np.asarray([], dtype=FRAME_DTYPE)
 
-        if config_frame_type4:
-            frame_arrays_on_core[core_coord] = np.concatenate(
-                [
-                    config_frame_type1.value,
-                    config_frame_type2.value,
-                    frame3,
-                    config_frame_type4.value,
-                ],
-                dtype=FRAME_DTYPE,
-                casting="no",
-            )
-        else:
-            frame_arrays_on_core[core_coord] = np.concatenate(
-                [config_frame_type1.value, config_frame_type2.value, frame3],
-                dtype=FRAME_DTYPE,
-                casting="no",
-            )
+            # 4. Only one config frame type IV for each physical core.
+            n_addr_write = v.params_reg.num_dendrite  # The number of address to write
+            if n_addr_write > 0:
+                config_frame_type4 = OfflineFrameGen.gen_config_frame4(
+                    chip_coord,
+                    core_coord,
+                    _default_rid,
+                    0,
+                    18 * n_addr_write,
+                    v.weight_ram[:n_addr_write],
+                )
+            else:
+                config_frame_type4 = None
+
+            _debug_dict[core_coord] = {
+                "config1": config_frame_type1,
+                "config2": config_frame_type2,
+                "config3": config_frame_type3,
+                "config4": config_frame_type4,
+            }
+
+            if config_frame_type4:
+                frame_arrays_on_core[core_coord] = np.concatenate(
+                    [
+                        config_frame_type1.value,
+                        config_frame_type2.value,
+                        frame3,
+                        config_frame_type4.value,
+                    ],
+                    dtype=FRAME_DTYPE,
+                    casting="no",
+                )
+            else:
+                frame_arrays_on_core[core_coord] = np.concatenate(
+                    [config_frame_type1.value, config_frame_type2.value, frame3],
+                    dtype=FRAME_DTYPE,
+                    casting="no",
+                )
 
     if write_to_file:
         if split_by_coord:
             for core_coord, f in frame_arrays_on_core.items():
                 addr = core_coord.address
                 _write_to_f(f"config_core{addr}", f)
         else:
@@ -415,45 +447,80 @@
                 list(frame_arrays_on_core.values()), dtype=FRAME_DTYPE, casting="no"
             )
             _write_to_f(f"config_cores_all", _f)
 
     return frame_arrays_on_core
 
 
-class PAIConfigJsonEncoder(json.JSONEncoder):
-    def default(self, o: Any) -> Any:
-        if isinstance(o, Coord):
-            return o.address
-        elif isinstance(o, Enum):
-            return o.value
-        elif isinstance(o, np.ndarray):
-            return o.tolist()
-        elif isinstance(o, NeuronDestInfo):
-            return o.model_dump(by_alias=True)
-        else:
-            return super().default(o)
-
-
-DEFAULT_CORE_PARAMS_CONF_JSON = "core_params.json"
-DEFAULT_INPUT_NODES_CONF_JSON = "input_proj_info.json"
-DEFAULT_OUTPUT_DESTS_CONF_JSON = "output_dest_info.json"
-
-
 def export_core_params_json(core_conf: Dict[Coord, CoreConfig], fp: Path) -> None:
-    _valid_conf = {k.address: v.__json__() for k, v in core_conf.items()}
-
-    with open(fp / DEFAULT_CORE_PARAMS_CONF_JSON, "w") as f:
-        json.dump(_valid_conf, f, ensure_ascii=True, indent=4, cls=PAIConfigJsonEncoder)
+    _valid_conf = {str(k): v.export() for k, v in core_conf.items()}
 
+    if _use_orjson:
+        with open(fp / _BACKEND_CONTEXT["core_conf_json"], "wb") as f:
+            f.write(
+                orjson.dumps(
+                    _valid_conf,
+                    option=orjson.OPT_NON_STR_KEYS | orjson.OPT_INDENT_2,
+                )
+            )
+    else:
+        with open(fp / _BACKEND_CONTEXT["core_conf_json"], "w") as f:
+            json.dump(
+                _valid_conf, f, ensure_ascii=True, indent=2, cls=PAIConfigJsonEncoder
+            )
 
-def export_inp_nodes_conf_json(inp_nodes_info: InputNodeInfo, fp: Path) -> None:
-    _valid_conf = {k: v.__json__() for k, v in inp_nodes_info.items()}
-
-    with open(fp / DEFAULT_INPUT_NODES_CONF_JSON, "w") as f:
-        json.dump(_valid_conf, f, ensure_ascii=True, indent=4, cls=PAIConfigJsonEncoder)
 
+def export_input_conf_json(input_conf_info: InputNodeConf, fp: Path) -> None:
+    _valid_conf = {k: v.export() for k, v in input_conf_info.items()}
 
-def export_outp_dests_conf_json(outp_dests_info: OutputDestInfo, fp: Path) -> None:
-    with open(fp / DEFAULT_OUTPUT_DESTS_CONF_JSON, "w") as f:
-        json.dump(
-            outp_dests_info, f, ensure_ascii=True, indent=4, cls=PAIConfigJsonEncoder
-        )
+    if _use_orjson:
+        with open(fp / _BACKEND_CONTEXT["input_conf_json"], "wb") as f:
+            f.write(orjson.dumps(_valid_conf, option=orjson.OPT_INDENT_2))
+    else:
+        with open(fp / _BACKEND_CONTEXT["input_conf_json"], "w") as f:
+            json.dump(_valid_conf, f, indent=2, cls=PAIConfigJsonEncoder)
+
+
+def export_output_conf_json(output_conf_info: OutputDestConf, fp: Path) -> None:
+    if _use_orjson:
+        with open(fp / _BACKEND_CONTEXT["output_conf_json"], "wb") as f:
+            f.write(
+                orjson.dumps(
+                    output_conf_info,
+                    default=PAIConfigJsonDefault,
+                    option=orjson.OPT_NON_STR_KEYS | orjson.OPT_INDENT_2,
+                )
+            )
+    else:
+        with open(fp / _BACKEND_CONTEXT["output_conf_json"], "w") as f:
+            json.dump(output_conf_info, f, indent=2, cls=PAIConfigJsonEncoder)
+
+
+def export_neuconf_json(neuron_conf: Dict[NeuDyn, NeuronConfig], full_fp: Path) -> None:
+    _valid_conf = {k.name: v.export() for k, v in neuron_conf.items()}
+
+    if _use_orjson:
+        with open(full_fp, "wb") as f:
+            f.write(orjson.dumps(_valid_conf, option=orjson.OPT_INDENT_2))
+    else:
+        with open(full_fp, "w") as f:
+            json.dump(_valid_conf, f, indent=2, cls=PAIConfigJsonEncoder)
+
+
+def export_core_plm_conf_json(core_plm_conf: CorePlmConf, full_fp: Path) -> None:
+    _valid_conf = {}
+
+    for chip_coord, cconf in core_plm_conf.items():
+        _valid_conf[str(chip_coord)] = {}
+        for core_coord, conf in cconf.items():
+            _valid_conf[str(chip_coord)][str(core_coord)] = conf.export()
+
+    if _use_orjson:
+        with open(full_fp, "wb") as f:
+            f.write(
+                orjson.dumps(
+                    _valid_conf, option=orjson.OPT_NON_STR_KEYS | orjson.OPT_INDENT_2
+                )
+            )
+    else:
+        with open(full_fp, "w") as f:
+            json.dump(_valid_conf, f, indent=2, cls=PAIConfigJsonEncoder)
```

### Comparing `paibox-1.0.0rc1/paibox/backend/constrs.py` & `paibox-1.1.0a1/paibox/backend/constrs.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0rc1/paibox/backend/context.py` & `paibox-1.1.0a1/paibox/backend/context.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,69 @@
 from pathlib import Path
-from typing import Any, Dict, Union
+from typing import Any, Dict, List, Union
 
-from paicorelib import Coord, CoordLike, to_coord
+from paicorelib import ChipCoord, Coord, CoordLike, to_coord
+from paicorelib.coordinate import to_coords
 
 from paibox.context import _Context
+from paibox.utils import merge_unique_ordered
 
-__all__ = ["BACKEND_CONFIG"]
+__all__ = []
 
 DEFAULT_OUTPUT_CHIP_ADDR = Coord(1, 0)
-DEFAULT_LOCAL_CHIP_ADDR = Coord(0, 0)
+DEFAULT_LOCAL_CHIP_ADDR = [Coord(0, 0)]  # Support multi-chip.
 DEFAULT_OUTPUT_CORE_ADDR_START = Coord(0, 0)
+DEFAULT_CORE_PARAMS_CONF_JSON = "core_params.json"
+DEFAULT_INPUT_CONF_JSON = "input_proj_info.json"
+DEFAULT_OUTPUT_CONF_JSON = "output_dest_info.json"
 
 
 class _BackendContext(_Context):
+    _DefaultContext = {
+        "output_chip_addr": DEFAULT_OUTPUT_CHIP_ADDR,  # RO mostly
+        "target_chip_addr": DEFAULT_LOCAL_CHIP_ADDR,  # RO mostly
+        "build_directory": Path.cwd(),  # R/W
+        "output_core_addr_start": DEFAULT_OUTPUT_CORE_ADDR_START,  # RO
+        "core_conf_json": DEFAULT_CORE_PARAMS_CONF_JSON,  # RO mostly
+        "input_conf_json": DEFAULT_INPUT_CONF_JSON,  # RO mostly
+        "output_conf_json": DEFAULT_OUTPUT_CONF_JSON,  # RO mostly
+        "cflags": dict(),  # R/W
+    }
+
     def __init__(self) -> None:
         super().__init__()
-        self["output_chip_addr"] = DEFAULT_OUTPUT_CHIP_ADDR  # RO mostly
-        self["local_chip_addr"] = DEFAULT_LOCAL_CHIP_ADDR  # RO mostly
-        self["build_directory"] = Path.cwd()  # R/W
-        self["output_core_addr_start"] = DEFAULT_OUTPUT_CORE_ADDR_START  # RO
-        self["cflags"] = dict()  # R/W
+        self.update(self._DefaultContext)
+
+    @property
+    def target_chip_addr(self) -> List[ChipCoord]:
+        return self["target_chip_addr"]
+
+    @target_chip_addr.setter
+    def target_chip_addr(self, addr: Union[CoordLike, List[CoordLike]]) -> None:
+        if isinstance(addr, list):
+            self["target_chip_addr"] = to_coords(addr)
+        else:
+            self["target_chip_addr"] = [to_coord(addr)]
+
+    def add_chip_addr(self, *chip_addrs: CoordLike) -> None:
+        # Maintain the order. We may take advantage of the priority
+        # of the chip coordinates later.
+        self["target_chip_addr"] = merge_unique_ordered(
+            self.target_chip_addr, to_coords(chip_addrs)
+        )
 
     @property
-    def local_chip_addr(self) -> Coord:
-        return self["local_chip_addr"]
+    def n_target_chips(self) -> int:
+        return len(self.target_chip_addr)
 
-    @local_chip_addr.setter
-    def local_chip_addr(self, addr: CoordLike) -> None:
-        self["local_chip_addr"] = to_coord(addr)
+    def _target_chip_addr_repr(self) -> str:
+        return ", ".join(str(a) for a in self.target_chip_addr)
 
     @property
-    def output_chip_addr(self) -> Coord:
+    def output_chip_addr(self) -> ChipCoord:
         return self["output_chip_addr"]
 
     @output_chip_addr.setter
     def output_chip_addr(self, addr: CoordLike) -> None:
         self["output_chip_addr"] = to_coord(addr)
 
     @property
@@ -56,13 +85,12 @@
     @property
     def cflags(self) -> Dict[str, Any]:
         """Compilation options."""
         return self["cflags"]
 
 
 _BACKEND_CONTEXT = _BackendContext()
-BACKEND_CONFIG = _BACKEND_CONTEXT
 
 
 def set_cflag(**kwargs) -> None:
     for k, v in kwargs.items():
         _BACKEND_CONTEXT.cflags[k] = v
```

### Comparing `paibox-1.0.0rc1/paibox/backend/graphs.py` & `paibox-1.1.0a1/paibox/backend/graphs.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,144 +7,166 @@
     Iterable,
     List,
     Mapping,
     Sequence,
     Set,
     Tuple,
     TypeVar,
+    Union,
 )
 
 from paicorelib import HwConfig
 
 from paibox.base import NeuDyn
 from paibox.collector import Collector
-from paibox.exceptions import BuildError, NotSupportedError
+from paibox.components import FullConnectedSyn, InputProj, NeuModule
+from paibox.exceptions import GraphBuildError, GraphConnectionError, NotSupportedError
 from paibox.network import DynSysGroup
-from paibox.projection import InputProj
-from paibox.synapses import SynSys
 
 from .constrs import GraphNodeConstrs
 from .graphs_types import *
 from .placement import CoreBlock
 from .routing import RoutingGroup
 
-_NT = TypeVar("_NT", CoreBlock, NodeName)
-
 
 @dataclass
 class PAIGraph:
     """Directed graph of PAIBox. We treat networks as one whole graph. \
         In the graph, synapses are edges while neurons are nodes.
     """
 
-    networks: Tuple[DynSysGroup, ...] = field(default_factory=tuple)
+    _raw_networks: Tuple[DynSysGroup, ...] = field(default_factory=tuple)
     """All networks are seen as one graph."""
+    _raw_nodes: Collector[NodeName, NodeType] = field(default_factory=Collector)
+    """Raw nodes in the networks."""
+    _raw_edges: Collector[EdgeName, EdgeType] = field(default_factory=Collector)
+    """Raw edges in the graph."""
+    _raw_fmodules: Collector[NodeName, NeuModule] = field(default_factory=Collector)
+    """Raw functional modules in the graph."""
+
     nodes: Dict[NodeName, NodeAttr] = field(default_factory=dict)
     """General nodes in the graph."""
     edges: Dict[EdgeName, EdgeAttr] = field(default_factory=dict)
     """General edges in the graph."""
 
     inodes: Collector[NodeName, SourceNodeType] = field(default_factory=Collector)
     """Input nodes in the graph."""
     onodes: Collector[NodeName, DestNodeType] = field(default_factory=Collector)
     """Output nodes in the graph."""
 
     ordered_nodes: List[NodeName] = field(default_factory=list)
-    """Ordered topologically nodes."""
+    """Nodes in topological sort order."""
 
     succ_dg: Dict[NodeName, Dict[NodeName, EdgeAttr]] = field(default_factory=dict)
     """Successor edges & nodes of every node in the graph."""
 
     degree_of_nodes: Dict[NodeName, NodeDegree] = field(default_factory=dict)
     """A dictionary of in/out-degree tuple of nodes."""
 
-    _raw_nodes: Collector[NodeName, NodeType] = field(default_factory=Collector)
-    """Raw nodes in the networks."""
-    _raw_edges: Collector[EdgeName, EdgeType] = field(default_factory=Collector)
-    """Raw edges in the graph."""
-
     """Status options"""
     has_built: bool = field(default=False)
 
     # node_constrs: GraphNodeConstrs = field(default_factory=GraphNodeConstrs)
 
-    def clear(self) -> None:
+    def clear(self, total: bool = True) -> None:
         """Clear the PAIGraph."""
         self.has_built = False
 
-        self.networks = ()
         self.nodes.clear()
         self.edges.clear()
         self.inodes.clear()
         self.onodes.clear()
         self.ordered_nodes.clear()
         self.succ_dg.clear()
         self.degree_of_nodes.clear()
 
-        self._raw_nodes.clear()
-        self._raw_edges.clear()
+        if total:
+            self._raw_networks = ()
+            self._raw_nodes.clear()
+            self._raw_edges.clear()
 
-        # self.node_constrs.clear()
-
-    def build(
-        self,
-        *networks: DynSysGroup,
-        # bounded_nodes: Sequence[Sequence[NeuDyn]] = (),
-        # conflicted_nodes: Dict[NodeName, Sequence[NeuDyn]] = {},
-    ) -> None:
+    def build(self, *networks: DynSysGroup, **build_options) -> None:
         self.clear()
-        self.networks = networks
 
-        _nodes: Collector[NodeName, NodeType] = Collector()
-        _edges: Collector[EdgeName, EdgeType] = Collector()
+        self._raw_networks = networks
+        self._pre_build(**build_options)
+
+        nodes: Collector[NodeName, NodeType] = Collector()
+        edges: Collector[EdgeName, EdgeType] = Collector()
+        fm: Collector[NodeName, NeuModule] = Collector()
+
+        for subnet in self._raw_networks:
+            fm += subnet.components.subset(NeuModule).unique()
+            nodes += (
+                subnet.components.include(InputProj, NeuDyn).exclude(NeuModule).unique()
+            )
+            edges += subnet.components.subset(FullConnectedSyn).unique()
+
+        self._raw_nodes += nodes.val_on_condition(
+            lambda node: not node.__gh_build_ignore__
+        )
+        self._raw_edges += edges.val_on_condition(
+            lambda edge: not edge.__gh_build_ignore__
+        )
+        self._raw_fmodules = fm
 
-        for network in networks:
-            sub_nodes = network.nodes(include_self=False, find_recursive=True)
-            _nodes += sub_nodes.include(InputProj, NeuDyn).unique()
-            _edges += sub_nodes.subset(SynSys).unique()
+        self._update_graph(**build_options)
 
-        self._raw_nodes = _nodes
-        self._raw_edges = _edges
+    def _pre_build(self, **build_options) -> None:
+        """Preprocessing before obtaining the topology."""
+        # Build functional modules in the subnets
+        for subnet in self._raw_networks:
+            DynSysGroup.build_fmodule(subnet, **build_options)
 
-        # Add all nodes in the graph.
-        for node in _nodes:
+    def _update_graph(self, **build_options) -> None:
+        self.clear(total=False)
+
+        # TODO Check isolated nodes in _raw_nodes
+        for node in self._raw_nodes:
             self.succ_dg[node] = dict()
 
         for syn in self._raw_edges.values():
             u, v = syn.source.name, syn.dest.name
-            # TODO tick_relative = 1 in default here.
-            self.succ_dg[u][v] = EdgeAttr(edge=syn, distance=1)
+            if u not in self._raw_nodes:
+                raise GraphConnectionError(
+                    f"the source neuron {u} of {syn.name} is not included in the graph."
+                )
+
+            if v not in self._raw_nodes:
+                raise GraphConnectionError(
+                    f"the dest neuron {v} of {syn.name} is not included in the graph."
+                )
+
+            self.succ_dg[u][v] = EdgeAttr(edge=syn, distance=syn.source.delay_relative)
 
         self.degree_of_nodes = get_node_degrees(self.succ_dg)
 
         # `InputProj` nodes are input nodes definitely.
-        self.inodes = _nodes.subset(InputProj)
+        self.inodes = self._raw_nodes.subset(InputProj)
 
         # By default, nodes with out-degree = 0 are considered as output nodes.
-        self.onodes = _nodes.key_on_condition(
+        self.onodes = self._raw_nodes.key_on_condition(
             lambda node: self.degree_of_nodes[node].out_degree == 0
-        )
+        )  # type: ignore
 
-        # _bounded_nodes_check(bounded_nodes)
-
-        for name, node in _nodes.items():
+        for name, node in self._raw_nodes.items():
             self.nodes[name] = NodeAttr(
                 node=node,
                 position=self._node_pos(name),
                 degree=self.degree_of_nodes[name],
             )
 
-        for name, syn in _edges.items():
+        for name, syn in self._raw_edges.items():
             self.edges[name] = EdgeAttr(edge=syn, distance=syn.source.delay_relative)
 
         self.has_built = True
 
-        self._graph_supported_check()
+        self._gh_support_check()
 
-    def _graph_supported_check(self) -> None:
+    def _gh_support_check(self) -> None:
         """Preprocess of the directed graph. Because there are currently    \
             many limitations on the networks that can be processed, checks  \
             are performed at this stage.
 
         Limitation:
             # For a node with in-degree > 1, the out-degree of all its      \
             #   forward nodes = 1.
@@ -186,15 +208,15 @@
         elif node in self.onodes:
             return NodePosition.OUTPUT
         else:
             return NodePosition.MEMBER
 
     def build_check(self) -> None:
         if not self.has_built:
-            raise BuildError(f"the graph hasn't been built yet.")
+            raise GraphBuildError(f"the graph hasn't been built yet.")
 
     def group_edges(self) -> Tuple[List[FrozenSet[EdgeType]], List[int]]:
         """Group all edges according to a certain rule.
 
         Return: a list of set of grouped edges and a list of routing groups id.
         """
         self.build_check()
@@ -280,20 +302,19 @@
         self.build_check()
         _, distance = get_longest_path(self.succ_dg, self.ordered_nodes)
 
         return distance
 
     @property
     def graph_name_repr(self) -> str:
-        _str = f"graph_of_{self.networks[0].name}"
+        _prefix = "graph_of_"
+        return _prefix + "_and_".join(network.name for network in self._raw_networks)
 
-        for network in self.networks[1:]:
-            _str += f"_and_{network.name}"
 
-        return _str
+_NT = TypeVar("_NT", CoreBlock, NodeName)
 
 
 def _degree_check(
     degree_of_nodes: Mapping[_NT, NodeDegree], succ_dg: Mapping[_NT, Iterable[_NT]]
 ) -> None:
     """Filter out such network structure, which is currently not supported."""
     for node in filter(lambda node: degree_of_nodes[node].out_degree > 1, succ_dg):
```

### Comparing `paibox-1.0.0rc1/paibox/backend/graphs_types.py` & `paibox-1.1.0a1/paibox/backend/graphs_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,21 +4,33 @@
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     from typing_extensions import TypeAlias
 
 from paibox.base import NeuDyn
-from paibox.projection import InputProj
-from paibox.synapses import SynSys
+from paibox.components import FullConnectedSyn, InputProj
+
+__all__ = [
+    "NodeName",
+    "EdgeName",
+    "NodeType",
+    "EdgeType",
+    "SourceNodeType",
+    "DestNodeType",
+    "NodePosition",
+    "NodeDegree",
+    "NodeAttr",
+    "EdgeAttr",
+]
 
 NodeName: TypeAlias = str
 EdgeName: TypeAlias = str
 NodeType: TypeAlias = Union[InputProj, NeuDyn]
-EdgeType: TypeAlias = SynSys
+EdgeType: TypeAlias = FullConnectedSyn
 SourceNodeType: TypeAlias = NodeType
 DestNodeType: TypeAlias = NeuDyn
 
 
 @unique
 class NodePosition(Enum):
     """Charactor of a node in the directed graph."""
```

### Comparing `paibox-1.0.0rc1/paibox/backend/mapper.py` & `paibox-1.1.0a1/paibox/backend/mapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,77 +1,64 @@
 import sys
 from collections import defaultdict
 from copy import copy
 from pathlib import Path
 from typing import Any, Dict, List, Literal, Optional, Union
 
-from paicorelib import (
-    Coord,
-    CoordLike,
-    CoordOffset,
-    HwConfig,
-    get_replication_id,
-    to_coord,
-)
+from paicorelib import Coord, CoordOffset, HwConfig, get_replication_id
 
 from paibox.base import NeuDyn, SynSys
-from paibox.exceptions import ResourceError
+from paibox.exceptions import ConfigInvalidError, ResourceError
 from paibox.network import DynSysGroup
 
 from .conf_template import (
     CoreConfig,
-    CorePlacementInfo,
+    CorePlmConf,
     GraphInfo,
-    InputNodeInfo,
+    InputNodeConf,
     NeuronDest,
-    OutputDestInfo,
+    OutputDestConf,
     export_core_params_json,
-    export_inp_nodes_conf_json,
-    export_outp_dests_conf_json,
+    export_input_conf_json,
+    export_output_conf_json,
     gen_config_frames_by_coreconf,
 )
 from .context import _BACKEND_CONTEXT, set_cflag
 from .graphs import PAIGraph, convert2routing_groups, get_node_degrees
 from .graphs_types import NodeDegree, SourceNodeType
 from .placement import CoreBlock, aligned_coords, max_lcn_of_cb
 from .routing import RoutingGroup, RoutingRoot
+from .segment_utils import NeuSeg
 
 __all__ = ["Mapper"]
 
 
 class Mapper:
-    """
-        Responsible for integrating all backend operation processes & \
-        providing functions for debugging.
-        TODO It doesn't collect information during the build process.
-    """
-
-    routing_tree = RoutingRoot(tag="L5")
-    """The routing tree root."""
     graph = PAIGraph()
+    graph_info: GraphInfo
 
     def __init__(self) -> None:
         self.core_blocks: List[CoreBlock] = []
         """List for core blocks in the network."""
         self.succ_core_blocks: Dict[CoreBlock, List[CoreBlock]] = defaultdict(list)
         self.input_core_blocks: Dict[SourceNodeType, List[CoreBlock]] = defaultdict(
             list
         )
         """List of input core blocks for each input node."""
 
         self.degrees_of_cb: Dict[CoreBlock, NodeDegree] = defaultdict(NodeDegree)
         self.routing_groups: List[RoutingGroup] = []
 
-        self.core_plm_config: CorePlacementInfo = dict()
+        self.core_plm_config: CorePlmConf = defaultdict(dict)
         self.core_params: Dict[Coord, CoreConfig] = dict()
         """The dictionary of core parameters."""
 
-        self.graph_info: GraphInfo
         self.n_core_required = 0
         self.n_core_occupied = 0
+        self.routing_tree = RoutingRoot(chip_list=_BACKEND_CONTEXT["target_chip_addr"])
 
         self.clear()
 
     def clear(self) -> None:
         self.routing_tree.clear()
         self.graph.clear()
 
@@ -86,33 +73,26 @@
         self.n_core_occupied = 0
 
         # Set default cflags
         _BACKEND_CONTEXT.cflags.clear()
         set_cflag(enable_wp_opt=True)
         set_cflag(grouping_optim_target="both")
 
-    def build(
-        self,
-        *networks: DynSysGroup,
-        # bounded_nodes: Sequence[Sequence[NeuDyn]] = (),
-        # conflicted_nodes: Dict[NodeName, Sequence[NeuDyn]] = {},
-    ) -> None:
-        """Build the directed graph based on given networks.    \
-            More than one networks in one graph is supported.
+    def build(self, *networks: DynSysGroup, **build_options) -> None:
+        """Build the directed graph based on given networks. More than one networks in one graph is supported.
 
         Args:
             - networks: one or many `DynSysGroup`.
 
-        TODO verify the following phases when more than one sub  \
-            network is given.
+        TODO verify the following phases when more than one sub network is given.
         """
         self.clear()
 
         # Filter & check the constraints to nodes.
-        self.graph.build(*networks)
+        self.graph.build(*networks, **build_options)
 
     def compile(
         self,
         *,
         weight_bit_optimization: Optional[bool] = None,
         grouping_optim_target: Optional[Literal["latency", "core", "both"]] = None,
     ) -> GraphInfo:
@@ -229,51 +209,49 @@
             else:
                 # Doesn't have following core blocks
                 cb.lcn_locked = True
 
     def coord_assign(self) -> None:
         """Assign the coordinate of each `CorePlacement`.
 
-        NOTE: The neurons in each core block must be grouped first to determine the #N of cores required,   \
-            and then the routing coordinates can be assigned.
+        NOTE: The neurons in each core block must be grouped first to determine the \
+            #N of cores required, and then the routing coordinates can be assigned.
         """
         for cb in self.core_blocks:
             # Group the neurons, get the #N of cores required.
             cb.group_neurons(
                 optim_target=_BACKEND_CONTEXT.cflags["grouping_optim_target"]
             )
 
         # Calculate the consumption of required physical cores.
+        n_avail_cores = HwConfig.N_CORE_OFFLINE * _BACKEND_CONTEXT.n_target_chips
         if (
             n_core_required := sum(cb.n_core_required for cb in self.core_blocks)
-        ) > HwConfig.N_CORE_OFFLINE:
+        ) > n_avail_cores:
             raise ResourceError(
-                f"the number of required cores is out of range {HwConfig.N_CORE_OFFLINE} ({n_core_required})."
+                CORE_RESOURCE_OUT_OF_RANGE_TEXT.format(n_avail_cores, n_core_required)
             )
 
         self.n_core_required = n_core_required
 
         # Generate routing groups by given the list of core blocks.
         routing_groups = convert2routing_groups(
             self.succ_core_blocks, self.degrees_of_cb, self.input_core_blocks
         )
         for rg in routing_groups:
-            if not self.routing_tree.insert_routing_group(rg):
-                raise RuntimeError(
-                    f"insert routing group {rg} into the routing tree failed."
-                )
+            self.routing_tree.insert_routing_group(rg)
 
         self.routing_groups = routing_groups
 
         # Calculate the consumption of occupied physical cores.
         if (
             n_core_occupied := sum(rg.get_n_core_occupied() for rg in routing_groups)
-        ) > HwConfig.N_CORE_OFFLINE:
+        ) > n_avail_cores:
             raise ResourceError(
-                f"the number of occupied cores is out of range {HwConfig.N_CORE_OFFLINE} ({n_core_occupied})."
+                CORE_RESOURCE_OUT_OF_RANGE_TEXT.format(n_avail_cores, n_core_occupied)
             )
 
         self.n_core_occupied = n_core_occupied
 
     def core_allocation(self) -> None:
         """Allocate the routing groups to core placements level."""
         for rg in self.routing_groups:
@@ -283,14 +261,22 @@
         """Export parameters of cores & neurons inside.
 
         Steps:
             - 1. Export the parameters(PARAMETER_REG, including RANDOM_SEED \
                 & Weight RAM) of cores.
             - 2. Export the parameters(Neuron RAM) of neurons inside.
         """
+        if (ochip_coord := _BACKEND_CONTEXT["output_chip_addr"]) in _BACKEND_CONTEXT[
+            "target_chip_addr"
+        ]:
+            raise ConfigInvalidError(
+                f"The output chip address  {ochip_coord} should not overlap with the "
+                f"chip addresses, but got {_BACKEND_CONTEXT._target_chip_addr_repr()}."
+            )
+
         input_nodes_info = self._inpproj_config_export()
         output_dest_info = self._member_cb_and_onode_config_export()
 
         _graph_info = GraphInfo(
             input=input_nodes_info,
             output=output_dest_info,
             members=self.core_plm_config,  # The configuration of physical cores is in `core_plm_config`
@@ -303,15 +289,15 @@
         self.graph_info = _graph_info
 
         return _graph_info
 
     def _set_global_cflags(self) -> None:
         SynSys.CFLAG_ENABLE_WP_OPTIMIZATION = _BACKEND_CONTEXT.cflags["enable_wp_opt"]
 
-    def _inpproj_config_export(self) -> InputNodeInfo:
+    def _inpproj_config_export(self) -> InputNodeConf:
         """Export the configuration of input projections.
 
         Json exchange file format for input nodes:
         {
             "inp1_1": { # as input node #1 without dest info
                 "addr_core_x": 0,
                 "addr_core_y": 0,
@@ -326,14 +312,16 @@
         }
         """
         input_nodes_info = dict()
 
         # Traverse input core blocks
         for inode, input_cbs in self.input_core_blocks.items():
             dest_coords: List[Coord] = []
+
+            assert all(input_cbs[0].chip_coord == cb.chip_coord for cb in input_cbs)
             for cb in input_cbs:  # Do not use iterative generation.
                 dest_coords.extend(cb.core_coords)
 
             dest_rid = get_replication_id(dest_coords)
 
             # The arrangement of axons is the same for the rest of `input_cbs`.
             # LCN of `input_cbs` are the same.
@@ -348,23 +336,23 @@
             neuron_dest = NeuronDest(
                 [coord.tick_relative for coord in axon_coords],
                 [coord.addr_axon for coord in axon_coords],
                 dest_coords[0].x,
                 dest_coords[0].y,
                 dest_rid.x,
                 dest_rid.y,
-                _BACKEND_CONTEXT["local_chip_addr"].x,
-                _BACKEND_CONTEXT["local_chip_addr"].y,
+                input_cb.chip_coord.x,
+                input_cb.chip_coord.y,
             )
 
             input_nodes_info[inode.name] = neuron_dest
 
         return input_nodes_info
 
-    def _member_cb_and_onode_config_export(self) -> OutputDestInfo:
+    def _member_cb_and_onode_config_export(self) -> OutputDestConf:
         """Export configuration & output destinations inormation for core blocks.
 
         Description:
             Traverse core placements in core blocks, find the following core    \
             blocks where the axons at. Get the coordinate of the core placement \
             & coordinates of axons(for multicasting).
 
@@ -407,62 +395,64 @@
                         member_cb, output_dest_info, ocoord
                     )
                 else:
                     # member_cb is a pure member.
                     self._member_cb_config_export(member_cb)
 
                 for coord, core_plm in member_cb.core_placements.items():
-                    self.core_plm_config[coord] = core_plm.export_core_plm_config()
+                    self.core_plm_config[rg.chip_coord][
+                        coord
+                    ] = core_plm.export_core_plm_config()
 
             # Generate default configurations for wasted core placements of the routing group
-            self.core_plm_config.update(rg.get_wasted_cplm_config())
+            self.core_plm_config[rg.chip_coord].update(rg.get_wasted_cplm_config())
 
         return output_dest_info
 
     def _member_cb_config_export(self, member_cb: CoreBlock) -> None:
         """Export configuration information for core blocks that are pure members."""
-        succ_cbs = self.succ_core_blocks[member_cb]
-
         for core_plm in member_cb.core_placements.values():
             for neu_seg in core_plm.neu_segs_of_cplm:
                 # Find the axon destinations of neu_seg, not the successor core blocks.
-                dest_cb_of_nseg = [cb for cb in succ_cbs if neu_seg.parent in cb.source]
+                dest_cb_of_nseg = self._find_dest_cb_by_nseg(neu_seg, member_cb)
 
-                assert _cb_routable(self.routing_groups, dest_cb_of_nseg)
-                core_plm.export_neu_config(neu_seg, dest_cb_of_nseg)
+                if len(dest_cb_of_nseg) > 0:
+                    assert _cb_routable(self.routing_groups, dest_cb_of_nseg)
+                    core_plm.export_neu_config(neu_seg, dest_cb_of_nseg)
+                else:
+                    raise ValueError(f"find destination of member {neu_seg} failed.")
 
     def _member_onode_cb_config_export(
         self,
         member_onode_cb: CoreBlock,
-        output_dest_info: OutputDestInfo,
+        output_dest_info: OutputDestConf,
         ocoord: Coord,
     ) -> Coord:
         """Export configuration information for core blocks that are both members & output."""
         cur_ocoord = ocoord
         output_axon_offset = 0
         o_nodes = [d for d in member_onode_cb.dest if d in self.graph.onodes.values()]
-        succ_cbs = self.succ_core_blocks[member_onode_cb]
 
         for core_plm in member_onode_cb.core_placements.values():
             for neu_seg in core_plm.neu_segs_of_cplm:
-                dest_cb_of_nseg = [cb for cb in succ_cbs if neu_seg.parent in cb.source]
+                dest_cb_of_nseg = self._find_dest_cb_by_nseg(neu_seg, member_onode_cb)
 
                 if len(dest_cb_of_nseg) > 0:
                     assert _cb_routable(self.routing_groups, dest_cb_of_nseg)
                     core_plm.export_neu_config(neu_seg, dest_cb_of_nseg)
                 else:
                     offset_idx = o_nodes.index(neu_seg.parent)
 
                     if hasattr(CoordOffset, "from_offset"):
                         # For paicorelib > 0.0.13
-                        raise NotImplementedError
+                        cur_ocoord = ocoord + CoordOffset.from_offset(offset_idx)
                     else:
                         # For paicorelib <= 0.0.13
                         cur_ocoord = ocoord + CoordOffset(
-                            offset_idx % 32, offset_idx // 32
+                            offset_idx // 32, offset_idx % 32
                         )
 
                     output_axon_offset = core_plm.export_neu_config(
                         neu_seg,
                         output_core_coord=cur_ocoord,
                         axon_addr_offset=output_axon_offset,
                     )
@@ -470,32 +460,32 @@
                         core_plm.neu_configs[neu_seg.parent].neuron_dest_info
                     )
 
         # Add the offset as the starting coordinate of the next output node
         return cur_ocoord + CoordOffset(1, 0)
 
     def _onode_cb_config_export(
-        self, onode_cb: CoreBlock, output_dest_info: OutputDestInfo, ocoord: Coord
+        self, onode_cb: CoreBlock, output_dest_info: OutputDestConf, ocoord: Coord
     ) -> Coord:
         """Export configuration information for core blocks that are pure output."""
         cur_ocoord = ocoord
         output_axon_offset = 0
         o_nodes = [d for d in onode_cb.dest if d in self.graph.onodes.values()]
 
         for core_plm in onode_cb.core_placements.values():
             for neu_seg in core_plm.neu_segs_of_cplm:
                 # Get the output coordinate of this neu_seg
                 offset_idx = o_nodes.index(neu_seg.parent)
 
                 if hasattr(CoordOffset, "from_offset"):
                     # For paicorelib > 0.0.13
-                    raise NotImplementedError
+                    cur_ocoord = ocoord + CoordOffset.from_offset(offset_idx)
                 else:
                     # For paicorelib <= 0.0.13
-                    cur_ocoord = ocoord + CoordOffset(offset_idx % 32, offset_idx // 32)
+                    cur_ocoord = ocoord + CoordOffset(offset_idx // 32, offset_idx % 32)
 
                 output_axon_offset = core_plm.export_neu_config(
                     neu_seg,
                     output_core_coord=cur_ocoord,
                     axon_addr_offset=output_axon_offset,
                 )
                 output_dest_info[neu_seg.parent.name][core_plm.coord.address] = (
@@ -506,58 +496,44 @@
 
     def export(
         self,
         write_to_file: bool = True,
         *,
         fp: Optional[Union[str, Path]] = None,
         format: Literal["txt", "bin", "npy"] = "bin",
-        split_by_coordinate: bool = False,
-        local_chip_addr: Optional[CoordLike] = None,
+        split_by_coord: bool = False,
         export_core_params: bool = False,
     ) -> Dict[Coord, Any]:
         """Generate configuration frames & export to file.
 
         Args:
             - write_to_file: whether to write frames into file.
             - fp: If `write_to_file` is `True`, specify the output path.
             - format: `txt`, `bin`, or `npy`. `bin` is recommended.
-            - split_by_coordinate: whether to split the generated frames file by the core coordinates.
-            - local_chip_addr: the address of the local chip. If not specified, the default value in    \
-                `_BACKEND_CONTEXT` will be used.
+            - split_by_coord: whether to split the generated frames file by the core coordinates.
             - export_core_params: whether to export the parameters of occupied cores.
 
         Return: a dictionary of configurations.
         """
         if format not in ("bin", "npy", "txt"):
             raise ValueError(f"format {format} is not supported.")
 
         _fp = _fp_check(fp)
-
-        if local_chip_addr is not None:
-            _local_chip_addr = to_coord(local_chip_addr)
-        else:
-            _local_chip_addr = _BACKEND_CONTEXT["local_chip_addr"]
-
         config_dict = gen_config_frames_by_coreconf(
-            self.graph_info["members"],
-            _local_chip_addr,
-            write_to_file,
-            _fp,
-            split_by_coordinate,
-            format,
+            self.graph_info["members"], write_to_file, _fp, split_by_coord, format
         )
 
         if export_core_params:
             # Export the parameters of occupied cores
             export_core_params_json(self.core_params, _fp)
 
-        # Export the info of input nodes
-        export_inp_nodes_conf_json(self.graph_info["input"], _fp)
-        # Export the info of output destinations
-        export_outp_dests_conf_json(self.graph_info["output"], _fp)
+        # Export the configurations of input nodes
+        export_input_conf_json(self.graph_info["input"], _fp)
+        # Export the configurations of output destinations
+        export_output_conf_json(self.graph_info["output"], _fp)
 
         return config_dict
 
     def find_neuron(self, neuron: NeuDyn, *, verbose: int = 0) -> None:
         self._build_check()
 
         for cb in self.core_blocks:
@@ -589,14 +565,20 @@
                     f"Address width:    {axon_segment.addr_width}\n"
                     f"Address offset:   {axon_segment.addr_offset}"
                 )
 
     def _build_check(self) -> None:
         return self.graph.build_check()
 
+    def _find_dest_cb_by_nseg(self, neu_seg: NeuSeg, cb: CoreBlock) -> List[CoreBlock]:
+        succ_cbs = self.succ_core_blocks[cb]
+        dest_cb_of_nseg = [cb for cb in succ_cbs if neu_seg.parent in cb.source]
+
+        return dest_cb_of_nseg
+
 
 def group_by(dict_: Dict, keyfunc=lambda item: item):
     """Groups the given list or dictionary by the value returned by ``keyfunc``."""
     d = defaultdict(list)
 
     for item in dict_.values():
         d[keyfunc(item)].append(item)
@@ -623,7 +605,12 @@
     else:
         _fp = _BACKEND_CONTEXT["build_directory"]
 
     if not _fp.is_dir():
         _fp.mkdir(parents=True, exist_ok=True)
 
     return _fp
+
+
+CORE_RESOURCE_OUT_OF_RANGE_TEXT = (
+    "the number of required cores is out of range {0} ({1})."
+)
```

### Comparing `paibox-1.0.0rc1/paibox/backend/placement.py` & `paibox-1.1.0a1/paibox/backend/placement.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,35 +12,30 @@
 else:
     from typing_extensions import TypeAlias
 
 from paicorelib import (
     LCN_EX,
     AxonCoord,
     AxonSegment,
+    ChipCoord,
     Coord,
     CoreMode,
     CoreModeDict,
     HwConfig,
     HwCore,
     MaxPoolingEnable,
 )
 from paicorelib import WeightPrecision as WP
 
-from paibox.base import NeuDyn, PAIBoxObject
-from paibox.exceptions import BuildError, ResourceError, TruncationWarning
-from paibox.synapses import SynSys
+from paibox.base import NeuDyn, PAIBoxObject, SynSys
+from paibox.exceptions import GraphBuildError, ResourceError, TruncationWarning
 from paibox.types import WeightType
 from paibox.utils import check_attr_same, count_unique_elem
 
-from .conf_template import (
-    CoreConfig,
-    CorePlacementConfig,
-    EmptyCorePlacementConfig,
-    NeuronConfig,
-)
+from .conf_template import CoreConfig, CorePlmConfig, EmptyCorePlmConfig, NeuronConfig
 from .context import _BACKEND_CONTEXT
 from .graphs_types import DestNodeType, SourceNodeType
 from .segment_utils import (
     NeuSeg,
     NeuSegOfCoreBlock,
     NeuSegOfCorePlm,
     aligned_coords,
@@ -71,29 +66,32 @@
             - routing_id: id of routing group.
             - seed: random seed. Default value is 0.
             - name: name of the core block. Optional.
         """
         super().__init__(name)
         self._parents = parents
         self._lcn_ex = self._n_axon2lcn_ex()
-        self._wp = WP.WEIGHT_WIDTH_8BIT  # Default value
+        self._wp = WP.WEIGHT_WIDTH_8BIT  # default value
         self._routing_id = routing_id
 
         self.seed = seed
         """Random seed, legal integer, no more than uint64."""
 
         self.target_lcn = LCN_EX.LCN_1X
         """The target(destination core block) LCN."""
 
         self.lcn_locked = False
         """Used to indicate whether `lcn_ex` has been adjusted."""
 
         self.core_coords: List[Coord] = list()
         """Assigned core coordinates."""
 
+        self.chip_coord: ChipCoord = Coord(0, 0)  # default
+        """A core block must be placed on a chip."""
+
         self.core_placements: Dict[Coord, CorePlacement] = dict()
         """Core placements."""
 
         # Segment the group of axons.
         self.axon_segments: Dict[SourceNodeType, AxonSegment] = get_axon_segments(
             self.axons, self.n_timeslot, self.n_fanin_max
         )
@@ -105,27 +103,27 @@
         """
 
     def group_neurons(
         self, optim_target: Literal["latency", "core", "both"] = "both"
     ) -> None:
         """Group the neurons to determine the #N of cores required."""
         if not self.lcn_locked:
-            raise BuildError("Group the neurons after lcn_ex is locked.")
+            raise GraphBuildError("Group the neurons after lcn_ex is locked.")
 
         self.neuron_segs_of_cb = get_neu_segments(
             self.dest,
             self.neuron_capacity,
             _neuron_repl_prop(self.n_weight_bits, self.n_timeslot),
             optim_target,
         )
 
     def core_plm_alloc(self) -> None:
         """Allocate `CoreBlock` to physical cores."""
         if not self.lcn_locked:
-            raise BuildError("Allocate core placements after lcn_ex is locked.")
+            raise GraphBuildError("Allocate core placements after lcn_ex is locked.")
 
         for i, coord in enumerate(self.core_coords):
             # assert self.get_raw_weight_of_coord(i)[0].shape[0] == self.n_axon
             self.core_placements[coord] = CorePlacement.build(self, i)
 
     def _get_syn_of(self, src: SourceNodeType, dest: DestNodeType) -> Optional[SynSys]:
         for syn in self.obj:
@@ -141,15 +139,15 @@
         """
         if self.n_axon < 1:
             raise ValueError(
                 f"the number of axons must be positive, but got {self.n_axon}."
             )
 
         if (
-            lcn := ((self.n_axon - 1) // self.n_fanin_max).bit_length()
+            lcn := int((self.n_axon - 1) // self.n_fanin_max).bit_length()
         ) > LCN_EX.LCN_64X:
             _max_n_axons = self.n_fanin_max * (1 << LCN_EX.LCN_64X)
             raise ResourceError(
                 f"required LCN extension out of range {LCN_EX.LCN_64X} ({lcn}). "
                 f"The number of axons must be <= {_max_n_axons}. "
                 f"But synapses {self._obj_repr()} have a total of {self.n_axon} axons."
             )
@@ -290,15 +288,15 @@
     @property
     def n_neuron_of_plm(self) -> List[int]:
         """A list of the #N of neurons on each `CorePlacement`.
 
         FIXME Different in SNN/ANN RUNTIME_MODE.
         """
         if len(self.core_coords) == 0:
-            raise BuildError(f"do this after coordinates assignment.")
+            raise GraphBuildError(f"do this after coordinates assignment.")
 
         # Get #N of neurons on each `CorePlacement` according to the
         # maximum address required of neuron segments on each `CorePlacement`.
         assert [] not in self.neuron_segs_of_cb  # TODO if it never happens, remove it.
 
         return [
             sum(seg.n_neuron for seg in neuron_segs)
@@ -584,45 +582,46 @@
         axon_addr_offset: int,
     ) -> int: ...
 
     def export_neu_config(
         self,
         neu_seg: NeuSeg,
         axon_dests: Optional[List[CoreBlock]] = None,
-        *,
         output_core_coord: Optional[Coord] = None,
         axon_addr_offset: Optional[int] = None,
     ) -> Optional[int]:
         """Export the neuron configuration."""
         if isinstance(axon_dests, list):
             axon_coords = aligned_coords(
                 neu_seg.segment.index,
                 axon_dests[0].axon_segments[neu_seg.parent],
                 neu_seg.parent.delay_relative,
                 axon_dests[0].n_timeslot,
             )
 
-            # Get all core coordinates then get the RID.
+            # Get all core coordinates and replication ids.
+            assert all(axon_dests[0].chip_coord == ad.chip_coord for ad in axon_dests)
+
             dest_core_coords = []
-            for axon_dest in axon_dests:
-                dest_core_coords.extend(axon_dest.core_coords)
+            for ad in axon_dests:
+                dest_core_coords.extend(ad.core_coords)
 
             config = NeuronConfig.encapsulate(
                 neu_seg.parent,
                 neu_seg.n_neuron,
                 neu_seg.segment.addr_ram,
                 neu_seg.segment.addr_offset,
                 axon_coords,
                 dest_core_coords,
-                # local chip coordinate for member nodes
-                _BACKEND_CONTEXT["local_chip_addr"],
+                axon_dests[0].chip_coord,
             )
 
             self.neu_configs[neu_seg.parent] = config
         else:
+            # neu_seg is a part of an output node
             assert isinstance(output_core_coord, Coord)
             assert isinstance(axon_addr_offset, int)
 
             axon_coords = [
                 AxonCoord(0, i)
                 for i in range(axon_addr_offset, axon_addr_offset + neu_seg.n_neuron)
             ]
@@ -638,18 +637,18 @@
                 _BACKEND_CONTEXT["output_chip_addr"],
             )
 
             self.neu_configs[neu_seg.parent] = config
 
             return axon_addr_offset + neu_seg.n_neuron
 
-    def export_core_plm_config(self) -> CorePlacementConfig:
+    def export_core_plm_config(self) -> CorePlmConfig:
         core_param = self.export_param_config()
 
-        return CorePlacementConfig.encapsulate(
+        return CorePlmConfig.encapsulate(
             self.parent.seed,
             self.weight_ram,
             core_param,
             self.neu_configs,
         )
 
     @property
@@ -750,30 +749,26 @@
             _mode_params[2],                    # snn_mode_en
             self._default_target_lcn,           # target_lcn
             _BACKEND_CONTEXT.test_chip_addr,    # test_chip_addr
         )
         # fmt: on
         return cb_config
 
-    def export_core_plm_config(self) -> EmptyCorePlacementConfig:
+    def export_core_plm_config(self) -> EmptyCorePlmConfig:
         core_param = self.export_param_config()
-        return EmptyCorePlacementConfig.encapsulate(core_param)
+        return EmptyCorePlmConfig.encapsulate(core_param)
 
     @classmethod
     def build(cls, coord: Coord):
         return cls(coord)
 
     @property
     def n_core_required(self):
         return 1
 
-    @property
-    def shape(self) -> Tuple[int, int]:
-        return (0, 0)
-
 
 def max_lcn_of_cb(cb: List[CoreBlock]) -> LCN_EX:
     """Find the max LCN extenion of previous grouped synapses"""
     return max(cb, key=lambda cb: cb.lcn_ex).lcn_ex
 
 
 def _neuron_repl_prop(nbits: int, ntimeslot: int) -> int:
```

### Comparing `paibox-1.0.0rc1/paibox/backend/routing.py` & `paibox-1.1.0a1/paibox/backend/routing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 from typing import Any, Dict, Iterator, List, Optional, Sequence, final
 
-from paicorelib import Coord, HwConfig
-from paicorelib.routing_defs import ROUTING_DIRECTIONS_IDX, RoutingCoord, RoutingCost
+from paicorelib import ChipCoord, Coord, HwConfig
+from paicorelib.routing_defs import ROUTING_DIRECTIONS_IDX as DIREC_IDX
+from paicorelib.routing_defs import RoutingCoord, RoutingCost
 from paicorelib.routing_defs import RoutingDirection as Direction
 from paicorelib.routing_defs import RoutingLevel as Level
 from paicorelib.routing_defs import RoutingStatus as Status
 from paicorelib.routing_defs import get_routing_consumption
 
-from paibox.exceptions import NotSupportedError
+from paibox.exceptions import ResourceError, RoutingError
 
-from .conf_template import CorePlacementInfo
+from .conf_template import CorePlmConfInChip
 from .placement import CoreBlock, CorePlacement, EmptyCorePlacement
 
 __all__ = ["RoutingGroup", "RoutingRoot"]
 
 
 class RoutingCluster:
     def __init__(
         self,
         level: Level,
-        data: Optional[CorePlacement] = None,
-        *,
         direction: Direction = Direction.ANY,
+        *,
+        data: Optional[CorePlacement] = None,
         status: Optional[Status] = None,
         tag: Optional[str] = None,
+        include_online: bool = False,
     ) -> None:
-        """Instance a tree cluster with `level`.
+        """Instance a tree cluster with `level` and `direction`.
         - For a Lx(>0)-level cluster, after created, the length of children is `node_capacity`.
         - For a L0-level cluster, it's a leaf.
 
         Args:
             - level: the cluster level.
             - data: the data hanging on the cluster. Optional.
             - direction: the direction of the cluster itself. Default is `Direction.ANY`.
             - tag: a tag for user to identify. Optional.
 
         Attributes:
             - level: the cluster level.
             - children: the children of the cluster.
-            - direction: the direction of the cluster iteself.
+            - d: the direction of the cluster, relative to its parent.
             - item: the data hanging on the cluster.
             - tag: a tag for user to identify.
-            - status: the status of the cluster. It's only for L0-level leaves.
-
-        NOTE: Do not add methods `__len__` & `__contains__`.
+            - status: the status of the cluster. Only for L0-level leaves.
         """
-        self._level = level
-        self._children: Dict[Direction, RoutingCluster] = dict()
-        self._direction = direction
+        self.level = level
+        self.children: Dict[Direction, RoutingCluster] = dict()
+        self.d = direction
         self.item = data
         self.tag = tag
+        self.include_online = include_online
 
         # Only set the attribute for L0-level cluster.
         if self.level == Level.L0:
             setattr(self, "status", status)
 
     def clear(self) -> None:
         """Clear the tree."""
@@ -62,80 +63,101 @@
             root.children.clear()
             if root.level == Level.L1:
                 return
 
             for child in root.children.values():
                 dfs(child)
 
-            return None
-
         if self.level > Level.L0:
             dfs(self)
 
-    def create_child(self, force: bool = False, **kwargs) -> Optional["RoutingCluster"]:
+    def create_child(self, **kwargs) -> Optional["RoutingCluster"]:
         """Create a child. If full, return None."""
         child = RoutingCluster(Level(self.level - 1), **kwargs)
 
-        if not self.add_child(child, force=force):
+        if not self.add_child(child):
             return None
 
         return child
 
     def add_child(
-        self, child: "RoutingCluster", method: str = "nearest", force: bool = False
+        self, child: "RoutingCluster", check_hit_online: bool = False
     ) -> bool:
         if self.level == Level.L0:
             # L0-level cluster cannot add child.
             raise AttributeError(f"L0-level cluster cannot add child.")
 
         if self.is_full():
             return False
 
-        # Traverse from X0Y0 to X1Y1.
-        for d in ROUTING_DIRECTIONS_IDX:
-            if d not in self.children:
-                return self.add_child_to(child, d, force)
+        for d in DIREC_IDX:
+            if d not in self:
+                return self.add_child_to(child, d, check_hit_online)
 
         return False
 
     def add_child_to(
-        self, child: "RoutingCluster", d: Direction, force: bool = False
+        self, child: "RoutingCluster", d: Direction, check_hit_online: bool = False
     ) -> bool:
         """Add a child cluster to a certain `direction`."""
         if self.level - child.level != 1:
             raise ValueError(f"Cannot skip more than 1 level.")
 
-        if not force and d in self.children:
+        if d in self:
             return False
 
-        child.direction = d
+        if d == Direction.X1Y1:
+            if self.include_online and check_hit_online:
+                return False
+            else:
+                child.include_online = True
+
+        # child.direction = d. Already done in `self[d]`(__setitem__).
         self[d] = child
 
         return True
 
+    def remove_child(
+        self,
+        d: Direction,
+        revert_direc: Direction = Direction.ANY,
+        strict: bool = False,
+    ) -> Optional["RoutingCluster"]:
+        child = self.children.pop(d, None)
+
+        if child is None:
+            if strict:
+                raise RoutingError(f"Removed child of {d} from {self} failed.")
+            else:
+                return None
+
+        # Revert the properties that were modified in the previous insertion.
+        child.include_online = False
+        child.d = revert_direc
+
+        return child
+
     def find_cluster_by_path(
         self, path: Sequence[Direction]
     ) -> Optional["RoutingCluster"]:
-        """Find the cluster by given a path of `Direction`.
+        """Find the cluster by given a routing path.
 
         Description:
-            Find by starting at this level based on the path provided. \
-            Take `path[0]` each time and then do a recursive search.
-
-        NOTE: The length of path <= the level of this cluster.
+            Find by starting at this level based on the routing path provided.
+            Take `path[0]` each time and do a recursive search.
         """
         if len(path) == 0:
             return self
 
         if len(path) > self.level:
             raise ValueError(
-                f"the length of the {path} should be less than or equal to level."
+                f"the length of path must be no more than {self.level}, but got {len(path)}."
             )
 
-        if path[0] not in self.children:
+        if path[0] not in self:
             return None
 
         sub_cluster = self[path[0]]
 
         if len(path) > 1:
             return sub_cluster.find_cluster_by_path(path[1:])
         else:
@@ -198,16 +220,16 @@
         if lx == self.level:
             if self.n_child_avail() >= n_child_avail:
                 return self
             else:
                 return None
 
         if not self.is_empty():
-            for d in ROUTING_DIRECTIONS_IDX:
-                if d in self.children:
+            for d in DIREC_IDX:
+                if d in self:
                     cluster = self[d]._find_lx_cluster_with_n_child_avail(
                         lx, n_child_avail, method
                     )
                     if cluster is not None:
                         return cluster
 
         child = self.create_child()
@@ -215,205 +237,196 @@
             return None
 
         return child._find_lx_cluster_with_n_child_avail(lx, n_child_avail, method)
 
     def add_subtree(
         self,
         subtree: "RoutingCluster",
-        method: str = "nearest",
+        check_hit_online: bool,
     ) -> bool:
         """Add the subtree's children to itself. If successful, return the added parent cluster."""
         if subtree.level > self.level:
-            raise ValueError
+            raise ValueError(
+                f"subtree's level {subtree.level} must be no more than the current level {self.level}."
+            )
 
         if subtree.level == self.level:
             sub_n_child = len(subtree.children)
             if self.n_child_avail() < sub_n_child:
                 return False
 
             if sub_n_child == 1:
-                self.add_child(subtree.children[Direction.X0Y0])
+                self.add_child(subtree[Direction.X0Y0], check_hit_online)
 
             elif sub_n_child == 2:
-                if len(self.children) == 0:
-                    if HwConfig.COORD_Y_PRIORITY:
-                        self.add_child_to(
-                            subtree.children[Direction.X0Y0], Direction.X0Y0
-                        )
-                        self.add_child_to(
-                            subtree.children[Direction.X0Y1], Direction.X0Y1
-                        )
-                    else:
-                        self.add_child_to(
-                            subtree.children[Direction.X0Y0], Direction.X0Y0
-                        )
-                        self.add_child_to(
-                            subtree.children[Direction.X0Y1], Direction.X1Y0
-                        )
-                else:
-                    if HwConfig.COORD_Y_PRIORITY:
-                        self.add_child_to(
-                            subtree.children[Direction.X0Y0], Direction.X1Y0
-                        )
-                        self.add_child_to(
-                            subtree.children[Direction.X0Y1], Direction.X1Y1
-                        )
-                    else:
-                        self.add_child_to(
-                            subtree.children[Direction.X0Y0], Direction.X0Y1
-                        )
-                        self.add_child_to(
-                            subtree.children[Direction.X0Y1], Direction.X1Y1
+                n_cur_child = len(self.children)
+                hit_online = False
+
+                for i in range(sub_n_child):
+                    success = self.add_child_to(
+                        subtree[DIREC_IDX[i]],
+                        DIREC_IDX[n_cur_child + i],
+                        check_hit_online,
+                    )
+                    hit_online |= not success
+
+                if hit_online:
+                    # If any of the subtrees fail to insert, the inserted subtrees are removed.
+                    for i in range(sub_n_child):
+                        removed = self.remove_child(
+                            DIREC_IDX[n_cur_child + i], DIREC_IDX[i], strict=False
                         )
 
+                    return False
+
             elif sub_n_child == 4:
-                self._children = subtree.children
+                if self.include_online and check_hit_online:
+                    return False
+
+                self.children = subtree.children
+                # Because the tree is inserted using depth-first order, when a node is
+                # encountered with no child, it must be on the far right.
+                self[Direction.X1Y1].include_online = True
+
             else:
-                # Only support 1, 2, & 4.
-                raise NotSupportedError(
-                    f"the number of {sub_n_child} child is not supported."
-                )
+                raise ValueError(f"the number of {sub_n_child} child is invalid.")
 
             return True
 
         if not self.is_empty():
-            for d in ROUTING_DIRECTIONS_IDX:
-                if d in self.children:
-                    flag = self[d].add_subtree(subtree, method)
+            for d in DIREC_IDX:
+                if d in self:
+                    flag = self[d].add_subtree(subtree, check_hit_online)
                     if flag:
-                        return flag
+                        return True
 
         child = self.create_child()
         if not child:
             return False
 
-        return child.add_subtree(subtree, method)
+        return child.add_subtree(subtree, check_hit_online)
 
     @classmethod
     def create_lx_full_tree(
         cls,
         lx: Level,
         d: Direction = Direction.X0Y0,
         root_tag: Optional[str] = None,
     ) -> "RoutingCluster":
-        root = RoutingCluster(lx, direction=d, tag=root_tag)
+        root = RoutingCluster(lx, d, tag=root_tag)
 
         if lx > Level.L1:
             for i in range(root.node_capacity):
                 child = cls.create_lx_full_tree(
-                    Level(lx - 1), ROUTING_DIRECTIONS_IDX[i], f"L{lx-1}_{i}"
+                    Level(lx - 1), DIREC_IDX[i], f"L{lx-1}_{i}"
                 )
                 if not root.add_child(child):
                     raise ValueError
 
         return root
 
     @classmethod
     def create_routing_tree(cls, lx: Level, n_branch: int) -> "RoutingCluster":
         """Create a routing tree with `n_branch` child.
 
         NOTE: When lx == L1, do not create the L0-level child. \
             WHen lx > L1, create the lx-1 level child.
         """
-        if lx == Level.L0 or n_branch < 0:
-            raise ValueError
+        if n_branch < 0 or n_branch > HwConfig.N_SUB_ROUTING_NODE:
+            raise ValueError(f"#N of branches out of range, got {n_branch}.")
+
+        if lx == Level.L0:
+            raise ValueError(f"do not create L0-level node directly.")
 
-        root = RoutingCluster(lx, direction=Direction.X0Y0)
+        root = RoutingCluster(lx, Direction.X0Y0)
 
         # Create `n_branch` children when lx > L1.
         if lx > Level.L1:
             for i in range(n_branch):
-                child = cls.create_lx_full_tree(
-                    Level(lx - 1), ROUTING_DIRECTIONS_IDX[i]
-                )
+                child = cls.create_lx_full_tree(Level(lx - 1), DIREC_IDX[i])
                 if not root.add_child(child):
-                    raise ValueError
+                    raise ValueError(f"add child {child} failed.")
 
         return root
 
     def add_L0_for_placing(self, data: Any = None, **kwargs) -> "RoutingCluster":
         """Add L0 cluster for placing in the routing tree.
 
         Args:
             - data: the data attached to the L0-level cluster.
             - kwargs: other arguments of the L0-level cluster, status, tag, etc.
         """
-        cluster = RoutingCluster(Level.L0, data, **kwargs)
+        cluster = RoutingCluster(Level.L0, data=data, **kwargs)
 
         L1_cluster = self._find_lx_cluster_with_n_child_avail(Level.L1, 1)
         if not L1_cluster:
-            raise RuntimeError("available L1 cluster not found.")
+            raise RoutingError("available L1 cluster not found.")
 
         if not L1_cluster.add_child(cluster):
-            raise RuntimeError(f"add child to L1 cluster failed.")
+            raise RoutingError(f"add child to L1 cluster failed.")
 
         return cluster
 
-    def find_clusters_at_level(
+    def find_lx_clusters(
         self, lx: Level, n_child_avail_low: int = 0
     ) -> List["RoutingCluster"]:
         """Find all clusters at a `lx` level with at least `n_child_avail_low` child clusters."""
         if lx > self.level:
-            raise ValueError
+            return []
 
         clusters = []
 
         def dfs_preorder(root: RoutingCluster) -> None:
             if root.level == lx:
                 if root.n_child_avail() >= n_child_avail_low:
                     clusters.append(root)
 
-                return
+                return None
 
-            for d in ROUTING_DIRECTIONS_IDX:
-                if d in root.children:
+            for d in DIREC_IDX:
+                if d in root:
                     dfs_preorder(root[d])
 
         dfs_preorder(self)
         return clusters
 
     def find_leaf_at_level(self, lx: Level) -> List["RoutingCluster"]:
         """Find clusters with no child at the `lx` level."""
         if lx == Level.L0:
             return []
 
-        return self.find_clusters_at_level(lx, self.node_capacity)
+        return self.find_lx_clusters(lx, self.node_capacity)
 
-    def breadth_of_lx_clusters(self, lx: Level) -> int:
+    def breadth_of_lx(self, lx: Level) -> int:
         """Get the number of clusters in the routing tree at the given level."""
-        clusters = self.find_clusters_at_level(lx, 0)
+        clusters = self.find_lx_clusters(lx, 0)
 
         return len(clusters)
 
-    def __getitem__(self, key: Direction) -> "RoutingCluster":
-        return self.children[key]
+    def __getitem__(self, d: Direction) -> "RoutingCluster":
+        return self.children[d]
 
-    def __setitem__(self, key: Direction, value: "RoutingCluster") -> None:
-        self._children[key] = value
+    def __setitem__(self, d: Direction, child: "RoutingCluster") -> None:
+        self.children[d] = child
+        child.d = d  # Set the direction of the child.
+
+    def __str__(self) -> str:
+        _name = id(self) if self.tag is None else self.tag
+        return f"tree {_name} at {self.d.name} at level {self.level}"
 
-    @property
-    def level(self) -> Level:
-        return self._level
+    def __iter__(self) -> Iterator[Direction]:
+        return self.children.__iter__()
+
+    def __contains__(self, d: Direction) -> bool:
+        return d in self.children
 
     @property
     def node_capacity(self) -> int:
         return HwConfig.N_SUB_ROUTING_NODE if self.level > Level.L0 else 0
 
-    @property
-    def children(self):
-        return self._children
-
-    @property
-    def direction(self) -> Direction:
-        return self._direction
-
-    @direction.setter
-    def direction(self, d: Direction) -> None:
-        self._direction = d
-
 
 class RoutingGroup(List[CoreBlock]):
     """Core blocks located within a routing group are routable.
 
     NOTE: Axon groups within a routing group are the same.
     """
 
@@ -422,34 +435,37 @@
         self.assigned_coords: List[Coord] = []
         """Assigned core coordinates in the routing group"""
         self.wasted_coords: List[Coord] = []
         """Wasted core coordinates in routing group"""
         self.wasted_core_plm: Dict[Coord, EmptyCorePlacement] = {}
         """Wasted core placements"""
 
-    def assign(self, assigned: List[Coord], wasted: List[Coord]) -> None:
+    def assign(
+        self, assigned: List[Coord], wasted: List[Coord], chip_coord: Coord
+    ) -> None:
         self.assigned_coords = assigned
         self.wasted_coords = wasted
 
         # Assign the coordinates to each core block inside the routing group.
         cur_i = 0
         for cb in self:
             n = cb.n_core_required
             cb.core_coords = assigned[cur_i : cur_i + n]
+            cb.chip_coord = chip_coord
             cur_i += n
 
     def core_block_alloc(self) -> None:
         for cb in self:
             cb.core_plm_alloc()
 
         # Allocate blank core placements for the wasted coordinates.
         for coord in self.wasted_coords:
             self.wasted_core_plm[coord] = EmptyCorePlacement.build(coord)
 
-    def get_wasted_cplm_config(self) -> CorePlacementInfo:
+    def get_wasted_cplm_config(self) -> CorePlmConfInChip:
         return {
             coord: core_plm.export_core_plm_config()
             for coord, core_plm in self.wasted_core_plm.items()
         }
 
     def get_n_core_occupied(self) -> int:
         """Get the #N of cores occupied by the routing group."""
@@ -480,98 +496,145 @@
     def routing_cost(self) -> RoutingCost:
         return get_routing_consumption(self.n_core_required)
 
     @property
     def routing_level(self) -> Level:
         return self.routing_cost.get_routing_level()
 
+    @property
+    def chip_coord(self) -> ChipCoord:
+        if not all(cb.chip_coord == self[0].chip_coord for cb in self):
+            raise RoutingError(
+                "Chip coordinates in the routing group is not consistent."
+            )
+
+        return self[0].chip_coord
+
 
 @final
-class RoutingRoot(RoutingCluster):
-    def __init__(self, **kwargs) -> None:
-        """Initialize a routing quadtree root(L5-level)."""
-        super().__init__(Level.L5, **kwargs)
-
-    def get_leaf_coord(self, cluster: "RoutingCluster") -> RoutingCoord:
-        """Return the routing coordinate of the cluster(must be a L0 leaf)."""
-        path = self.get_routing_path(cluster)
+class RoutingRoot:
+    def __init__(self, chip_list: List[ChipCoord], **kwargs) -> None:
+        """Initialize a routing quadtree root."""
+        self.chip_list = chip_list
+        # Every L5 routing cluster is unique in each chip root.
+        self.chip_roots = [
+            RoutingCluster(Level.L5, include_online=True) for _ in range(len(chip_list))
+        ]
+
+    def get_leaf_coord(
+        self, root: RoutingCluster, leaf: RoutingCluster
+    ) -> RoutingCoord:
+        """Return the routing coordinate of the L0 leaf."""
+        path = root.get_routing_path(leaf)
         if path:
             return RoutingCoord(*path)
 
-        raise RuntimeError(f"get leaf cluster {cluster.tag} coordinate failed.")
+        raise RoutingError(f"get leaf {leaf.tag} coordinate failed.")
 
     def insert_routing_group(self, routing_group: RoutingGroup) -> bool:
         """Insert a `RoutingGroup` in the routing tree. Assign each core blocks with \
             routing coordinates & make sure they are routable.
 
         NOTE: Use depth-first search to insert each core block into the routing tree \
             to ensure that no routing deadlock occurs between core blocks.
         """
         cost = routing_group.routing_cost
         level = routing_group.routing_level
+        if cost.n_L0 > HwConfig.N_CORE_OFFLINE:
+            raise ResourceError(
+                f"the number of cores required exceeds the hardware limit, {cost.n_L0} > {HwConfig.N_CORE_OFFLINE}."
+            )
+
         # Create a routing cluster
         routing_cluster = RoutingCluster.create_routing_tree(level, cost[level - 1])
 
         # `n_L0` physical cores will be occupied.
         #   - For the first `n_core_required` cores, they are used for placement.
         #   - For the rest, they are unused.
         # Make sure the routing cluster is successfully inserted to the root
         # then assign coordinates & status.
         leaves = []
         wasted = []
         for i in range(cost.n_L0):
             if i < routing_group.n_core_required:
-                cluster = routing_cluster.add_L0_for_placing(
+                l0 = routing_cluster.add_L0_for_placing(
                     data=f"{id(routing_group)}_{i}",
                     status=Status.USED,
                     tag=f"{id(routing_group)}_{i}",
                 )
-                leaves.append(cluster)
+                leaves.append(l0)
 
             else:
-                cluster = routing_cluster.add_L0_for_placing(
+                l0 = routing_cluster.add_L0_for_placing(
                     status=Status.OCCUPIED, tag=f"{id(routing_group)}_{i}"
                 )
-                wasted.append(cluster)
+                wasted.append(l0)
+
+        # If #N of wasted cores > 16, it won't hit online L2 cluster.
+        check_hit_online = len(wasted) <= HwConfig.N_CORE_ONLINE
 
         # Add the sub-tree to the root.
-        flag = self.add_subtree(routing_cluster)
+        flag = False
+        # TODO For now, use sequential attempt.
+        for chip_coord, chip_root in zip(self.chip_list, self.chip_roots):
+            flag = chip_root.add_subtree(routing_cluster, check_hit_online)
+            if flag:
+                break
+
         if not flag:
-            return False
+            raise RoutingError(
+                f"insert routing group {routing_group} into the routing tree failed, "
+                f"cannot insert to any chip."
+            )
 
+        # TODO Consider obtaining the root coord of the `routing_cluster` applied for when inserting,
+        # and calculate all leaf coords according to the size of the routing group. Instead of
+        # recording all the leaves and then looking up their coordinates in the tree.
         valid_coords = []
         wasted_coords = []
         for cluster in leaves:
-            coord = self.get_leaf_coord(cluster)
-            valid_coords.append(coord.coordinate)
+            coord = self.get_leaf_coord(chip_root, cluster)
+            valid_coords.append(coord.to_coord())
 
         for cluster in wasted:
-            coord = self.get_leaf_coord(cluster)
-            wasted_coords.append(coord.coordinate)
+            coord = self.get_leaf_coord(chip_root, cluster)
+            wasted_coords.append(coord.to_coord())
 
-        routing_group.assign(valid_coords, wasted_coords)
+        routing_group.assign(valid_coords, wasted_coords, chip_coord)
 
         return True
 
-    @property
-    def n_L0_clusters(self) -> int:
-        return self.breadth_of_lx_clusters(Level.L0)
+    def clear(self) -> None:
+        for root in self:
+            root.clear()
+
+    def breadth_of_lx_at(self, lx: Level, chip_idx: int) -> int:
+        return self[chip_idx].breadth_of_lx(lx)
+
+    def breadth_of_lx(self, lx: Level) -> int:
+        return sum(chip_root.breadth_of_lx(lx) for chip_root in self)
+
+    def __getitem__(self, index: int) -> RoutingCluster:
+        return self.chip_roots[index]
+
+    def __iter__(self) -> Iterator[RoutingCluster]:
+        return self.chip_roots.__iter__()
 
 
 def get_parent(
     tree: RoutingCluster, cluster: RoutingCluster
 ) -> Optional[RoutingCluster]:
     """Get the parent cluster of the given cluster. If not found, return None."""
     assert tree != cluster
 
     def dfs_preorder(
         tree: RoutingCluster, cluster: RoutingCluster
     ) -> Optional[RoutingCluster]:
-        for d in ROUTING_DIRECTIONS_IDX:
-            if d in tree.children:
+        for d in DIREC_IDX:
+            if d in tree:
                 if tree[d] is cluster:
                     return tree
                 else:
                     parent = dfs_preorder(tree[d], cluster)
                     if parent:
                         return parent
```

### Comparing `paibox-1.0.0rc1/paibox/backend/segment_utils.py` & `paibox-1.1.0a1/paibox/backend/segment_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,17 @@
     def n_neuron(self) -> int:
         return self.segment.n_neuron
 
     @property
     def n_addr(self) -> int:
         return self.segment.n_addr
 
+    def __str__(self) -> str:
+        return f"NeuSeg {self.parent.name} at offset {self.segment.addr_offset}"
+
 
 NeuSlice: TypeAlias = slice
 NeuSegOfCorePlm: TypeAlias = List[NeuSeg]
 NeuSegOfCoreBlock: TypeAlias = List[NeuSegOfCorePlm]
 
 
 def _place_seperately(
@@ -253,19 +256,22 @@
 
 def get_neu_segments(
     neu_groups: List[NeuDyn],
     capacity: int,
     repl_prop: int,
     optim_target: Literal["latency", "core", "both"],
 ) -> NeuSegOfCoreBlock:
-    """Get the neuron segments by given a optimization strategy.
+    """Get the neuron segments with a optimization strategy.
 
     Args:
-        - optim_target: Target of optimization. 'catagory' strategy intends to optimize the throughput  \
-            of nodes. The 'dense' strategy intends to optimize the consumption of cores.
+        - neu_groups: group of neurons in the core block.
+        - capacity: #N of neurons that can be accommodated in a core.
+        - repl_prop: the proportion of neuron replication.
+        - optim_target: optimization target. 'latency' strategy intends to optimize the latency of nodes. \
+            'core' strategy intends to optimize the consumption of cores.
     """
     if optim_target == "core":
         seg_slices_dict = _get_neu_slices_opt_core(neu_groups, capacity)
         return _get_nsg_opt_core(seg_slices_dict, capacity, repl_prop)
 
     else:
         seg_slices_dict = _get_neu_slices_opt_latency(neu_groups, capacity)
```

### Comparing `paibox-1.0.0rc1/paibox/base.py` & `paibox-1.1.0a1/paibox/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 
 _IdPathType: TypeAlias = Tuple[int, int]
 
 
 class PAIBoxObject:
     _excluded_vars = ()
+    __avoid_name_conflict__: ClassVar[bool] = False
 
     def __init__(self, name: Optional[str] = None) -> None:
         self._name: str = self.unique_name(name)
 
     def __eq__(self, other: "PAIBoxObject") -> bool:
         if not isinstance(other, PAIBoxObject):
             raise TypeError(
@@ -49,15 +50,15 @@
             if _type is None:
                 __type = self.__class__.__name__
             else:
                 __type = _type
 
             return get_unique_name(__type)
 
-        is_name_unique(name, self)
+        is_name_unique(name, self, self.__avoid_name_conflict__)
         return name
 
     @property
     def name(self) -> str:
         return self._name
 
     @name.setter
@@ -215,14 +216,18 @@
     if path not in _paths:
         _paths.add(path)
         gather[v.name] = v
         nodes.append(v)
 
 
 class DynamicSys(PAIBoxObject, StatusMemory):
+    __gh_build_ignore__: bool = False
+    """To indicate whether the backend will take the object into account
+        when the network topology information is first constructed"""
+
     def __init__(self, name: Optional[str] = None) -> None:
         super().__init__(name)
         super(PAIBoxObject, self).__init__()
 
     def __call__(self, *args, **kwargs):
         raise NotImplementedError
 
@@ -281,15 +286,14 @@
             if sys.version_info >= (3, 9):
                 params.update({k.removeprefix("_"): v})
             else:
                 params.update({k.lstrip("_"): v})  # compatible for py3.8
 
         return params
 
-    @property
     def is_working(self) -> bool:
         return (self.tick_wait_start > 0 and self.timestamp >= 0) and (
             self.tick_wait_end == 0 or self.timestamp + 1 <= self.tick_wait_end
         )
 
     @property
     def delay_relative(self) -> int:
@@ -301,22 +305,22 @@
 
     @property
     def tick_wait_end(self) -> int:
         return self._twe
 
     @property
     def unrolling_factor(self) -> int:
-        return self._unrolling_factor
+        return self._uf
 
     @unrolling_factor.setter
     def unrolling_factor(self, factor: int) -> None:
         if factor < 1:
             raise ValueError(f"'unrolling_factor' must be positive, but got {factor}.")
 
-        self._unrolling_factor = factor
+        self._uf = factor
 
 
 class SynSys(DynamicSys):
     CFLAG_ENABLE_WP_OPTIMIZATION: ClassVar[bool] = True
     """Compilation flag for weight precision optimization."""
 
     @property
```

### Comparing `paibox-1.0.0rc1/paibox/collector.py` & `paibox-1.1.0a1/paibox/collector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,66 @@
-from typing import Callable, Dict, Generic, Sequence, Type, TypeVar, Union, overload
+from typing import (
+    Callable,
+    Dict,
+    MutableMapping,
+    Sequence,
+    Type,
+    TypeVar,
+    Union,
+    overload,
+)
 
 _T = TypeVar("_T")
 _KT = TypeVar("_KT")
 _VT = TypeVar("_VT")
 
+# XXX: use collections.UserDict[_KT, _VT] in 3.9+
 
-class Collector(dict, Generic[_KT, _VT]):
-    def __setitem__(self, key: _KT, value: _VT) -> None:
+
+class Collector(Dict[_KT, _VT]):
+    def __setitem__(self, key, value) -> None:
         if key in self:
             if id(self[key]) != id(value):
                 raise ValueError(
                     f"mame '{key}' conflicts: same name for {value} & {self[key]}."
                 )
 
         super().__setitem__(key, value)
 
-    def replace(self, key: _KT, new_value: _VT) -> None:
-        self.pop(key)
-        self.key = new_value
-
     @overload
-    def update(self, other: Dict[_KT, _VT]) -> "Collector[_KT, _VT]": ...
+    def update(self, other: MutableMapping[_KT, _VT]) -> "Collector[_KT, _VT]": ...
 
     @overload
     def update(self, other: Sequence[_T]) -> "Collector[_KT, _T]": ...
 
     def update(
-        self, other: Union[Dict[_KT, _VT], Sequence[_T]]
+        self, other: Union[MutableMapping[_KT, _VT], Sequence[_T]]
     ) -> Union["Collector[_KT, _VT]", "Collector[_KT, _T]"]:
-        if not isinstance(other, (dict, list, tuple)):
+        if not isinstance(other, (MutableMapping, list, tuple)):
             raise TypeError(
-                f"expected a dict, list or sequence, but got {other}, type {type(other)}."
+                f"expected a collector, dict, list or sequence, but got {other}, type {type(other)}."
             )
 
-        if isinstance(other, dict):
-            for k, v in other.items():
-                self[k] = v
+        if isinstance(other, MutableMapping):
+            super().update(other)
         else:
             l = len(self)
             for i, v in enumerate(other):
                 self[f"_{l+i}"] = v  # type: ignore
 
         return self
 
     @overload
-    def __add__(self, other: Dict[_KT, _VT]) -> "Collector[_KT, _VT]": ...
+    def __add__(self, other: MutableMapping[_KT, _VT]) -> "Collector[_KT, _VT]": ...
 
     @overload
     def __add__(self, other: Sequence[_T]) -> "Collector[_KT, _T]": ...
 
     def __add__(
-        self, other: Union[Dict[_KT, _VT], Sequence[_T]]
+        self, other: Union[MutableMapping[_KT, _VT], Sequence[_T]]
     ) -> Union["Collector[_KT, _VT]", "Collector[_KT, _T]"]:
         """Merging two dicts.
 
         Arguments:
             - other: the other dictionary.
 
         Returns:
@@ -62,30 +68,30 @@
         """
         gather = type(self)(self)
         gather.update(other)
 
         return gather
 
     @overload
-    def __sub__(self, other: Dict[_KT, _VT]) -> "Collector[_KT, _VT]": ...
+    def __sub__(self, other: MutableMapping[_KT, _VT]) -> "Collector[_KT, _VT]": ...
 
     @overload
     def __sub__(self, other: Sequence[_T]) -> "Collector[str, _T]": ...
 
     def __sub__(
-        self, other: Union[Dict[_KT, _VT], Sequence[_T]]
+        self, other: Union[MutableMapping[_KT, _VT], Sequence[_T]]
     ) -> Union["Collector[_KT, _VT]", "Collector[str, _T]"]:
-        if not isinstance(other, (dict, list, tuple)):
+        if not isinstance(other, (MutableMapping, list, tuple)):
             raise TypeError(
-                f"expected a dict, list or sequence, but got {other}, type {type(other)}."
+                f"expected a collector, dict, list or sequence, but got {other}, type {type(other)}."
             )
 
         gather = type(self)(self)
 
-        if isinstance(other, dict):
+        if isinstance(other, MutableMapping):
             for k, v in other.items():
                 if k not in gather.keys():
                     raise ValueError(f"cannot find '{k}' in {self.keys()}.")
 
                 if id(v) != id(gather[k]):
                     raise ValueError(
                         f"cannot remove '{k}', since there are two different values: "
@@ -112,71 +118,63 @@
                 if k not in gather:
                     raise KeyError(f"key '{k}' not found. Removed failed.")
 
                 gather.pop(k)
 
         return gather
 
-    def subset(self, obj_type: Type[_T]) -> "Collector":
-        gather = type(self)()
+    def subset(self, obj_type: Type[_T]) -> "Collector[_KT, _T]":
+        gather = Collector()
 
         for k, v in self.items():
             if isinstance(v, obj_type):
-                gather[k] = v  # type: ignore
+                gather[k] = v
 
         return gather
 
-    def not_subset(self, obj_type: Type[_T]) -> "Collector":
+    def not_subset(self, obj_type: Type[_T]) -> "Collector[_KT, _VT]":
         gather = type(self)()
 
         for k, v in self.items():
             if not isinstance(v, obj_type):
                 gather[k] = v
 
         return gather
 
-    def include(self, *types: Type[_T]) -> "Collector":
-        gather = type(self)()
+    def include(self, *types: Type[_T]) -> "Collector[_KT, _T]":
+        gather = Collector()
 
         for k, v in self.items():
             if isinstance(v, types):
-                gather[k] = v  # type: ignore
+                gather[k] = v
 
         return gather
 
-    def exclude(self, *types: Type[_T]) -> "Collector":
+    def exclude(self, *types: Type[_T]) -> "Collector[_KT, _VT]":
         gather = type(self)()
 
         for k, v in self.items():
             if not isinstance(v, types):
                 gather[k] = v
 
         return gather
 
-    def unique(self) -> "Collector":
+    def unique(self) -> "Collector[_KT, _VT]":
         gather = type(self)()
         seen = set()
 
         for k, v in self.items():
             if id(v) not in seen:
                 seen.add(id(v))
                 gather[k] = v
 
         return gather
 
-    def key_on_condition(self, condition: Callable[..., bool]) -> "Collector":
-        gather = type(self)()
-
-        for k, v in self.items():
-            if condition(k):
-                gather[k] = v
-
-        return gather
-
-    def value_on_condition(self, condition: Callable[..., bool]) -> "Collector":
-        gather = type(self)()
-
-        for k, v in self.items():
-            if condition(v):
-                gather[k] = v
-
-        return gather
+    def key_on_condition(
+        self, condition: Callable[[_KT], bool]
+    ) -> "Collector[_KT, _VT]":
+        return type(self)({k: v for k, v in self.items() if condition(k)})
+
+    def val_on_condition(
+        self, condition: Callable[[_VT], bool]
+    ) -> "Collector[_KT, _VT]":
+        return type(self)({k: v for k, v in self.items() if condition(v)})
```

### Comparing `paibox-1.0.0rc1/paibox/context.py` & `paibox-1.1.0a1/paibox/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from typing import Any, Generic, TypeVar
+from typing import Any, Dict, TypeVar
 
 __all__ = ["FRONTEND_ENV"]
 
 
 _KT = TypeVar("_KT")
 _VT = TypeVar("_VT")
 
+# XXX: use collections.UserDict[_KT, _VT] in 3.9+
 
-class _Context(dict, Generic[_KT, _VT]):
+
+class _Context(Dict[_KT, _VT]):
     def load(self, key: Any, default: Any = None) -> Any:
         """Load the context by the `key`.
 
         Args:
             - key: the key to indicate the data.
             - default: the default value when `key` is not defined.
         """
@@ -31,21 +33,15 @@
             )
 
         for i in range(0, len(args), 2):
             k = args[i]
             v = args[i + 1]
             super().__setitem__(k, v)
 
-        self.update(kwargs)  # compatible for py3.8
-
-    def __setitem__(self, key: Any, value: Any) -> None:
-        self.save(key, value)
-
-    def __getitem__(self, key: Any) -> Any:
-        return self.load(key)
+        self.update(**kwargs)  # compatible for py3.8
 
     def get_ctx(self):
         """Get all contexts."""
         return self.copy()
 
     def clear_ctx(self, *args) -> None:
         """Clear one or some contexts."""
```

### Comparing `paibox-1.0.0rc1/paibox/mixin.py` & `paibox-1.1.0a1/paibox/mixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from copy import deepcopy
 from functools import wraps
 from typing import Any, Dict, Optional, Sequence, Type, TypeVar
 
 import numpy as np
-from numpy.typing import NDArray
-
-import paibox as pb
 
 from .context import _FRONTEND_CONTEXT
 from .exceptions import RegisterError
 from .naming import get_unique_name
 from .node import NodeDict
+from .types import VoltageType
 
 _T = TypeVar("_T")
 
 
 def singleton(cls):
     instances = {}
 
@@ -59,25 +57,28 @@
 
 class MixIn:
     """Mix-in class."""
 
     pass
 
 
+# XXX this class seems useless
 class Container(MixIn):
     children: NodeDict[str, Any]
 
     def __getitem__(self, item: str) -> Any:
         if item in self.children:
             return self.children[item]
 
         raise KeyError(f"key '{item}' not found.")
 
-    def _get_elem_name(self, elem: object) -> str:
-        if isinstance(elem, pb.base.PAIBoxObject):
+    def _get_elem_name(self, elem: Any) -> str:
+        from .base import PAIBoxObject
+
+        if isinstance(elem, PAIBoxObject):
             return elem._name
         else:
             return get_unique_name("ContainerElem")
 
     def elem_format(
         self,
         child_type: Type[_T],
@@ -138,17 +139,17 @@
             return self.master_nodes.pop(key, None)
         elif strict:
             raise KeyError(f"key '{key}' not found in master nodes.")
 
     def get_master_node(self, key: str) -> Optional[Any]:
         return self.master_nodes.get(key, None)
 
-    def sum_inputs(self, **kwargs) -> NDArray[np.int32]:
+    def sum_inputs(self, *, init: VoltageType = 0, **kwargs) -> VoltageType:  # type: ignore
         # TODO Out is a np.ndarray right now, but it may be more than one type.
-        output = 0
+        output = init
         for node in self.master_nodes.values():
             output += node.output.copy()
 
         return np.array(output).astype(np.int32)
 
 
 class TimeRelatedNode(MixIn):
```

### Comparing `paibox-1.0.0rc1/paibox/naming.py` & `paibox-1.1.0a1/paibox/naming.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,39 @@
+import typing
 import warnings
 
 from .exceptions import PAIBoxWarning, RegisterError
 
 global _id_dict, _type_names
 _id_dict = dict()
 _type_names = dict()
 
 
-def is_name_unique(name: str, obj: object) -> None:
-    """If the name is unique, record it in the global dictionary.
-    Otherwise raise an error.
-    """
+if typing.TYPE_CHECKING:
+    from .base import PAIBoxObject
+
+
+def is_name_unique(name: str, obj: "PAIBoxObject", avoid: bool) -> None:
+    """If the name is unique, record it in the global dictionary."""
     if not name.isidentifier():
         raise ValueError(f"'{name}' is not a valid identifier.")
-
     if name in _id_dict:
         if _id_dict[name] != id(obj):
-            raise RegisterError(
-                f"name of {obj}({name}) is already used by {_id_dict[name]}."
-            )
-
+            if avoid:
+                new_name = name + "_1"
+                warnings.warn(
+                    f"name of {obj}({name}) is already used by {_id_dict[name]}, "
+                    f"change name to avoid: {name} -> {new_name}.",
+                    PAIBoxWarning,
+                )
+                return is_name_unique(new_name, obj, avoid=True)
+            else:
+                raise RegisterError(
+                    f"name of {obj}({name}) is already used by {_id_dict[name]}."
+                )
     else:
         _id_dict[name] = id(obj)
 
 
 def get_unique_name(_type: str) -> str:
     """Generate a unique name for a given type."""
     if _type not in _type_names:
```

### Comparing `paibox-1.0.0rc1/paibox/neuron/base.py` & `paibox-1.1.0a1/paibox/components/neuron/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,28 +209,28 @@
             if self.reset_mode is RM.MODE_NORMAL:
                 return np.full((self._n_neuron,), self.reset_v, dtype=np.int32)
 
             elif self.reset_mode is RM.MODE_LINEAR:
                 return np.subtract(
                     vjt, self.pos_threshold + self._v_th_rand, dtype=np.int32
                 )
-            else:
+            else:  # RM.MODE_NONRESET
                 return vjt
 
         def _when_exceed_neg() -> VoltageType:
             if self.neg_thres_mode is NTM.MODE_RESET:
                 if self.reset_mode is RM.MODE_NORMAL:
                     return np.full((self._n_neuron,), -self.reset_v, dtype=np.int32)
                 elif self.reset_mode is RM.MODE_LINEAR:
                     return np.add(
                         vjt,
                         self.neg_threshold + self._v_th_rand,
                         dtype=np.int32,
                     )
-                else:
+                else:  # RM.MODE_NONRESET
                     return vjt
 
             else:
                 return np.full((self._n_neuron,), -self.neg_threshold, dtype=np.int32)
 
         # USE "=="!
         v_reset = np.where(
@@ -368,15 +368,15 @@
         self,
         shape: Shape,
         reset_mode: RM = RM.MODE_NORMAL,
         reset_v: int = 0,
         leak_comparison: LCM = LCM.LEAK_AFTER_COMP,
         threshold_mask_bits: int = 0,
         neg_thres_mode: NTM = NTM.MODE_RESET,
-        neg_threshold: int = -1,
+        neg_threshold: int = 0,
         pos_threshold: int = 1,
         leak_direction: LDM = LDM.MODE_FORWARD,
         leak_integration_mode: LIM = LIM.MODE_DETERMINISTIC,
         leak_v: int = 0,
         synaptic_integration_mode: SIM = SIM.MODE_DETERMINISTIC,
         bit_truncation: int = 0,
         *,
@@ -459,15 +459,15 @@
                 (HwConfig.N_TIMESLOT_MAX,) + self._inner_spike.shape, dtype=np.bool_
             ),
         )
 
         self._delay = delay
         self._tws = tick_wait_start
         self._twe = tick_wait_end
-        self._unrolling_factor = unrolling_factor
+        self._uf = unrolling_factor
 
         """Counter of copies."""
         self._n_copied = 0
 
     def __len__(self) -> int:
         return self._n_neuron
 
@@ -478,15 +478,15 @@
 
     def update(
         self, x: Optional[np.ndarray] = None, *args, **kwargs
     ) -> Optional[SpikeType]:
         # Priority order is a must.
         # The neuron doesn't work if `tws = 0` & done working
         # until `t - tws + 1 > twe` under the condition `twe > 0`.
-        if not self.is_working:
+        if not self.is_working():
             self._inner_spike = self.init_param(0).astype(np.bool_)
             return None
 
         # The neuron is going to work.
         if x is None:
             x = self.sum_inputs()
```

### Comparing `paibox-1.0.0rc1/paibox/neuron/neurons.py` & `paibox-1.1.0a1/paibox/components/neuron/neurons.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,138 +2,126 @@
 
 from paicorelib import LCM, LDM, NTM, RM
 
 from paibox.types import Shape
 
 from .base import Neuron
 
+__all__ = ["IF", "LIF", "TonicSpiking", "PhasicSpiking", "Always1Neuron", "SpikingRelu"]
 
-class IF(Neuron):
-    """IF neuron"""
 
+class IF(Neuron):
     def __init__(
         self,
         shape: Shape,
         threshold: int,
         reset_v: int = 0,
         *,
         keep_shape: bool = False,
         name: Optional[str] = None,
         **kwargs,
     ) -> None:
-        """
+        """IF neuron.
+
         Arguments:
             - shape: shape of neurons.
             - threshold: when the membrane potential exceeds the threshold, neurons will fire.
             - reset_v: reset membrane potential after firing
             - delay: delay between neurons. Default is 1.
-            - tick_wait_start: set the neuron group to start at the `N`-th timestep. 0 means not to     \
-                start. Default is 1.
-            - tick_wait_end: set the neuron group to continue working for `M` timesteps, 0 means working\
-                forever. Default is 0.
-            - unrolling_factor: the argument is related to the backend. It means that neurons will be   \
-                unrolled & deployed to more physical cores to reduce latency and increase throughput.   \
-                Default is 1.
-            - keep_shape: whether to maintain size information when recording data in the simulation.   \
+            - tick_wait_start: set the moodule to start at timestep `T`. 0 means not working. Default is 1.
+            - tick_wait_end: set the module to turn off at time `T`. 0 means always working. Default is 0.
+            - unrolling_factor: argument related to the backend. It represents the degree to which modules  \
+                are expanded. The larger the value, the more cores required for deployment, but the lower   \
+                the latency & the higher the throughput. Default is 1.
+            - keep_shape: whether to maintain size information when recording data in the simulation.       \
                 Default is `False`.
-            - name: name of the object.
+            - name: name of the neuron. Optional.
         """
         super().__init__(
             shape,
             reset_v=reset_v,
             neg_thres_mode=NTM.MODE_SATURATION,
-            neg_threshold=0,
             pos_threshold=threshold,
             keep_shape=keep_shape,
             name=name,
             **kwargs,
         )
 
 
 class LIF(Neuron):
-    """LIF neuron"""
-
     def __init__(
         self,
         shape: Shape,
         threshold: int,
         reset_v: int = 0,
         leak_v: int = 0,
         *,
         keep_shape: bool = False,
         name: Optional[str] = None,
         **kwargs,
     ) -> None:
-        """
+        """LIF neuron.
+
         Arguments:
             - shape: shape of neurons.
             - threshold: when the membrane potential exceeds the threshold, neurons will fire.
             - reset_v: reset membrane potential after firing
             - leak_v: the signed leak voltage will be added directly to the membrane potential.
                 - If it is positive, the membrane potential will increase.
                 - If is is negative, the membrane potential will decrease.
         """
         super().__init__(
             shape,
             reset_mode=RM.MODE_NORMAL,
             reset_v=reset_v,
             neg_thres_mode=NTM.MODE_SATURATION,
-            neg_threshold=0,
             pos_threshold=threshold,
             leak_v=leak_v,
             keep_shape=keep_shape,
             name=name,
             **kwargs,
         )
 
 
 class TonicSpiking(Neuron):
-    """Tonic spiking neuron"""
-
     def __init__(
         self,
         shape: Shape,
         fire_step: int,
         *,
         keep_shape: bool = False,
         name: Optional[str] = None,
         **kwargs,
     ) -> None:
-        """
+        """Tonic spiking neuron.
+
         Arguments:
             - shape: shape of neurons.
             - fire_step: every `N` spike, the neuron will fire positively.
 
         NOTE: The neuron receives `N` spikes and fires, then it will reset to 0.
         """
         super().__init__(
-            shape,
-            neg_thres_mode=NTM.MODE_SATURATION,
-            neg_threshold=0,
-            pos_threshold=fire_step,
-            keep_shape=keep_shape,
-            name=name,
-            **kwargs,
+            shape, pos_threshold=fire_step, keep_shape=keep_shape, name=name, **kwargs
         )
 
 
 class PhasicSpiking(Neuron):
-    """Phasic spiking neuron"""
-
     def __init__(
         self,
         shape: Shape,
         time_to_fire: int,
         neg_floor: int = -10,
         *,
         keep_shape: bool = False,
         name: Optional[str] = None,
         **kwargs,
     ) -> None:
-        """
+        """Phasic spiking neuron.
+
         Arguments:
             - shape: shape of neurons.
             - time_to_fire: after `N` spikes, the neuron will fire positively.
             - neg_floor: once fired, the neurons will remain at this negative membrane potential.   \
                 Default is -10.
 
         NOTE: Once the neuron receives `N` spikes and fires, it will reset to the negative floor &  \
@@ -152,33 +140,44 @@
             keep_shape=keep_shape,
             name=name,
             **kwargs,
         )
 
 
 class Always1Neuron(Neuron):
-    """This neuron will always output 1 as long as it starts working.
-
-    FIXME There must be a forward synapse connected to it, otherwise    \
-        the backend will go wrong.
-    """
 
     def __init__(
         self,
         shape: Shape,
         *,
         keep_shape: bool = False,
         name: Optional[str] = None,
         **kwargs,
     ) -> None:
+        """A neuron that always outputs 1 as long as it starts working.
+
+        FIXME There must be a forward synapse connected to it, otherwise the backend will go wrong.
+        """
         super().__init__(
             shape,
             reset_v=1,
             leak_comparison=LCM.LEAK_BEFORE_COMP,
             neg_thres_mode=NTM.MODE_SATURATION,
-            neg_threshold=0,
             pos_threshold=0,
             leak_v=(1 << 29) - 1,
             keep_shape=keep_shape,
             name=name,
             **kwargs,
         )
+
+
+class SpikingRelu(Neuron):
+    def __init__(
+        self,
+        shape: Shape,
+        *,
+        keep_shape: bool = False,
+        name: Optional[str] = None,
+        **kwargs,
+    ) -> None:
+        """Spiking relu neuron. Act exactly the way you think."""
+        super().__init__(shape, keep_shape=keep_shape, name=name, **kwargs)
```

### Comparing `paibox-1.0.0rc1/paibox/neuron/utils.py` & `paibox-1.1.0a1/paibox/components/neuron/utils.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0rc1/paibox/projection.py` & `paibox-1.1.0a1/paibox/components/projection.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 import numpy as np
 
 if sys.version_info >= (3, 10):
     from typing import ParamSpec
 else:
     from typing_extensions import ParamSpec
 
-from .base import DynamicSys
-from .context import _FRONTEND_CONTEXT
-from .exceptions import ShapeError, SimulationError
-from .mixin import TimeRelatedNode
-from .types import DataType, Shape, SpikeType
-from .utils import as_shape, shape2num
+from paibox.base import DynamicSys
+from paibox.context import _FRONTEND_CONTEXT
+from paibox.exceptions import ShapeError, SimulationError
+from paibox.mixin import TimeRelatedNode
+from paibox.types import DataType, Shape, SpikeType
+from paibox.utils import as_shape, shape2num
 
 __all__ = ["InputProj"]
 
 P = ParamSpec("P")
 
 
 def _func_bypass(x: DataType) -> DataType:
```

### Comparing `paibox-1.0.0rc1/paibox/simulator/encoder.py` & `paibox-1.1.0a1/paibox/simulator/encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import math
 from typing import Any, Literal, Optional
 
 import numpy as np
 from numpy.typing import NDArray
 
+from paibox.components.synapses.conv_types import _KOrder4d, _Size2Type
+from paibox.components.synapses.conv_utils import _pair
 from paibox.mixin import StatusMemory
-from paibox.synapses.conv_utils import _KOrder4d, _pair, _Size2Type
 from paibox.types import SpikeType
 
 from .utils import _conv2d_faster_fp32
 
 __all__ = ["LatencyEncoder", "PeriodicEncoder", "PoissonEncoder", "Conv2dEncoder"]
 
 """
```

### Comparing `paibox-1.0.0rc1/paibox/simulator/probe.py` & `paibox-1.1.0a1/paibox/simulator/probe.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 from typing import Optional
 
 from paibox.base import PAIBoxObject
 
+__all__ = ["Probe"]
+
 
 class Probe(PAIBoxObject):
+    __avoid_name_conflict__ = True
+    target: PAIBoxObject
+
     def __init__(
         self,
         target: PAIBoxObject,
         attr: str,
         *,
         name: Optional[str] = None,
     ) -> None:
         """
         Arguments:
-            - target: the main target.
-            - attr: the attribute to probe.
+            - target: the target that needs to be monitored.
+            - attr: the attribute that needs to be monitored.
             - name: the name of the probe. Optional.
         """
-        super().__init__(name)
-
-        self.target: PAIBoxObject
         self.attr = attr
         self._check_attr(target)
 
+        super().__init__(name)
+
     def _check_attr(self, target: PAIBoxObject) -> None:
         if not hasattr(target, self.attr):
             raise AttributeError(
-                f"attribute '{self.attr}' not found in target {self.target}."
+                f"attribute '{self.attr}' not found in target {target}."
             )
 
         self.target = target
 
+    @property
+    def _label_txt(self) -> str:
+        return f" '{self.name}'" if hasattr(self, "name") else ""
+
     def __str__(self) -> str:
-        label_txt = f" '{self.name}'"
-        return f"<Probe{label_txt} of '{self.attr}' of {self.target}>"
+        return f"<Probe{self._label_txt} of '{self.attr}' of {self.target}>"
 
     def __repr__(self) -> str:
-        label_txt = f" '{self.name}'"
-        return f"<Probe{label_txt} at 0x{id(self):x} of '{self.attr}' of {self.target}>"
+        return f"<Probe{self._label_txt} at 0x{id(self):x} of '{self.attr}' of {self.target}>"
```

### Comparing `paibox-1.0.0rc1/paibox/simulator/simulator.py` & `paibox-1.1.0a1/paibox/simulator/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,16 @@
         self.reset()
 
     def run(self, duration: int, reset: bool = False, **kwargs) -> None:
         """
         Arguments:
             - duration: duration of the simulation.
             - reset: whether to reset the state of components in the model. Default is `False`.
-            - kwargs：determined by the parameter format of the input node. Will be deprecated.
+            - kwargs：determined by the parameter format of the input node. It will be deprecated, \
+                please use 'FRONTEND_ENV.save()' instead.
         """
         if kwargs:
             warnings.warn(
                 "passing extra arguments through 'run()' will be deprecated. "
                 "Use 'FRONTEND_ENV.save()' instead.",
                 DeprecationWarning,
             )
@@ -161,16 +162,19 @@
         for probe in self.probes:
             t = getattr(probe.target, probe.attr)
             data = t.copy() if hasattr(t, "copy") else copy.copy(t)  # Shallow copy
 
             self._sim_data[probe].append(data)
 
     def _add_inner_probes(self) -> None:
+        # Find probes at all levels.
         probe_nodes = (
-            self.target.nodes(level=1, include_self=False).subset(Probe).unique()
+            self.target.nodes(include_self=False, find_recursive=True)
+            .subset(Probe)
+            .unique()
         )
 
         for probe in probe_nodes.values():
             # Store the probe instances
             self.probes.append(probe)
             self._sim_data[probe] = []
```

### Comparing `paibox-1.0.0rc1/paibox/simulator/utils.py` & `paibox-1.1.0a1/paibox/simulator/utils.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0rc1/paibox/synapses/base.py` & `paibox-1.1.0a1/paibox/components/synapses/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from typing import ClassVar, Optional, Tuple, Union
 
 import numpy as np
 from paicorelib import HwConfig
 from paicorelib import WeightPrecision as WP
 
 from paibox.base import NeuDyn, SynSys
-from paibox.exceptions import ShapeError
-from paibox.neuron import Neuron
-from paibox.projection import InputProj
+from paibox.exceptions import RegisterError, ShapeError
 from paibox.types import DataArrayType, SynOutType, WeightType
 
-from .conv_utils import _fm_ndim1_check, _fm_ndim2_check, _KOrder3d, _KOrder4d
+from ..modules import BuildingModule
+from ..neuron import Neuron
+from ..projection import InputProj
+from .conv_types import _KOrder3d, _KOrder4d
+from .conv_utils import _fm_ndim1_check, _fm_ndim2_check
 from .transforms import (
     AllToAll,
     Conv1dForward,
     Conv2dForward,
     ConvTranspose1dForward,
     ConvTranspose2dForward,
 )
@@ -34,72 +36,115 @@
 
 
 class Synapses:
     def __init__(
         self,
         source: Union[NeuDyn, InputProj],
         dest: NeuDyn,
+        subclass_syn_name: str,
     ) -> None:
         self._source = source
-        self._dest = dest
+        self._target = dest
+        self._child_syn_name = subclass_syn_name
+        """The name of subclass `FullConnectedSyn`."""
 
     @property
     def source(self) -> Union[NeuDyn, InputProj]:
         return self._source
 
+    @source.setter
+    def source(self, source: Union[NeuDyn, InputProj]) -> None:
+        """Set a new source neuron."""
+        if source.num_out != self.num_in:
+            raise RegisterError(
+                f"the number of source neurons before and after the change"
+                f"is not equal: {source.num_out} != {self.num_in}."
+            )
+
+        self._source = source
+
     @property
     def dest(self) -> NeuDyn:
-        return self._dest
+        return self._target
+
+    @dest.setter
+    def dest(self, dest: NeuDyn) -> None:
+        """Set a new destination neuron."""
+        if dest.num_in != self.num_out:
+            raise RegisterError(
+                f"the number of source neurons before and after the change"
+                f"is not equal: {dest.num_in} != {self.num_out}."
+            )
+
+        self._target = dest
+        # FIXME Because the modification of the synapse destination neuron occurs in the backend,
+        # there's no need to register new dest again because simulation will not be done again (maybe).
+        # But does it mean that we need to make a copy of the original network and then pass it to
+        # the backend?
+        dest.register_master(
+            RIGISTER_MASTER_KEY_FORMAT.format(self._child_syn_name), self
+        )
+
+    @property
+    def target(self) -> NeuDyn:
+        return self._target
 
     @property
     def shape_in(self) -> Tuple[int, ...]:
         return self._source.shape_out
 
     @property
     def shape_out(self) -> Tuple[int, ...]:
-        return self._dest.shape_in
+        return self._target.shape_in
 
     @property
     def num_in(self) -> int:
         return self._source.num_out
 
     @property
     def num_out(self) -> int:
-        return self._dest.num_in
+        return self._target.num_in
 
 
 class FullConnectedSyn(Synapses, SynSys):
+
+    comm: Transform
+
     def __init__(
         self,
         source: Union[NeuDyn, InputProj],
         dest: NeuDyn,
         name: Optional[str] = None,
     ) -> None:
         super(Synapses, self).__init__(name)
-        super().__init__(source, dest)
+        super().__init__(source, dest, self.name)
 
         self.set_memory("_synout", np.zeros((self.num_out,), dtype=np.int32))
 
-        # Register `self` for the destination `NeuDyn`.
+        # Register itself with the master nodes of destination.
         dest.register_master(RIGISTER_MASTER_KEY_FORMAT.format(self.name), self)
 
+        # If the source is `BuildingModule`, register itself with its module interface.
+        if isinstance(source, BuildingModule):
+            source.register_output(self)
+
     def __call__(self, *args, **kwargs) -> SynOutType:
         return self.update(*args, **kwargs)
 
     def update(self, spike: Optional[np.ndarray] = None, *args, **kwargs) -> SynOutType:
         # Retrieve the spike at index `timestamp` of the dest neurons
-        if self.dest.is_working:
+        if self.dest.is_working():
             if isinstance(self.source, InputProj):
                 synin = self.source.output.copy() if spike is None else spike
             else:
                 idx = self.dest.timestamp % HwConfig.N_TIMESLOT_MAX
                 synin = self.source.output[idx].copy() if spike is None else spike
         else:
             # Retrieve 0 to the dest neurons if it is not working
-            synin = np.zeros_like(self.source.spike, dtype=np.bool_)
+            synin = np.zeros_like(self.source.spike)
 
         self._synout = self.comm(synin).ravel().astype(np.int32)
         return self._synout
 
     def reset_state(self, *args, **kwargs) -> None:
         # TODO Add other initialization methods in the future.
         self.reset_memory()  # Call reset of `StatusMemory`.
@@ -162,14 +207,15 @@
     def __init__(
         self,
         source: Union[NeuDyn, InputProj],
         dest: Neuron,
         kernel: np.ndarray,
         stride: Tuple[int],
         padding: Tuple[int],
+        dilation: Tuple[int],
         order: _KOrder3d,
         name: Optional[str] = None,
     ) -> None:
         super().__init__(source, dest, name)
 
         if kernel.ndim != self._spatial_ndim + 2:
             raise ShapeError(
@@ -181,37 +227,40 @@
         else:
             _kernel = kernel.copy()
 
         # O,I,L
         out_channels, in_channels, kernel_l = _kernel.shape
         # C,L
         in_ch, in_l = _fm_ndim1_check(source.shape_out, "CL")
-        out_l = (in_l + 2 * padding[0] - kernel_l) // stride[0] + 1
+        out_l = (in_l + 2 * padding[0] - dilation[0] * (kernel_l - 1) - 1) // stride[
+            0
+        ] + 1
 
         if in_ch != in_channels:
             raise ShapeError(f"input channels mismatch: {in_ch} != {in_channels}.")
 
         if (_output_size := out_channels * out_l) != dest.num_in:
             raise ShapeError(f"Output size mismatch: {_output_size} != {dest.num_in}.")
 
         comm = Conv1dForward((in_l,), (out_l,), _kernel, stride, padding)
 
-        self.comm = comm
+        self._set_comm(comm)
 
 
 class Conv2dSyn(FullConnectedSyn):
     _spatial_ndim: ClassVar[int] = 2
 
     def __init__(
         self,
         source: Union[NeuDyn, InputProj],
         dest: Neuron,
         kernel: np.ndarray,
         stride: Tuple[int, int],
         padding: Tuple[int, int],
+        dilation: Tuple[int, int],
         order: _KOrder4d,
         name: Optional[str] = None,
     ) -> None:
         super().__init__(source, dest, name)
 
         if kernel.ndim != self._spatial_ndim + 2:
             raise ShapeError(
@@ -223,16 +272,20 @@
         else:
             _kernel = kernel.copy()
 
         # O,I,H,W
         out_channels, in_channels, kernel_h, kernel_w = _kernel.shape
         # C,H,W
         in_ch, in_h, in_w = _fm_ndim2_check(source.shape_out, "CHW")
-        out_h = (in_h + 2 * padding[0] - kernel_h) // stride[0] + 1
-        out_w = (in_w + 2 * padding[1] - kernel_w) // stride[1] + 1
+        out_h = (in_h + 2 * padding[0] - dilation[0] * (kernel_h - 1) - 1) // stride[
+            0
+        ] + 1
+        out_w = (in_w + 2 * padding[1] - dilation[1] * (kernel_w - 1) - 1) // stride[
+            1
+        ] + 1
 
         if in_ch != in_channels:
             raise ShapeError(f"input channels mismatch: {in_ch} != {in_channels}.")
 
         if (_output_size := out_channels * out_h * out_w) != dest.num_in:
             raise ShapeError(f"Output size mismatch: {_output_size} != {dest.num_in}.")
 
@@ -247,14 +300,15 @@
     def __init__(
         self,
         source: Union[NeuDyn, InputProj],
         dest: Neuron,
         kernel: np.ndarray,
         stride: Tuple[int],
         padding: Tuple[int],
+        dilation: Tuple[int],
         output_padding: Tuple[int],
         order: _KOrder3d,
         name: Optional[str] = None,
     ) -> None:
         super().__init__(source, dest, name)
 
         if kernel.ndim != self._spatial_ndim + 2:
@@ -267,39 +321,46 @@
         else:
             _kernel = kernel.copy()
 
         # O,I,L
         out_channels, in_channels, kernel_l = _kernel.shape
         # C,L
         in_ch, in_l = _fm_ndim1_check(source.shape_out, "CL")
-        out_l = (in_l - 1) * stride[0] - 2 * padding[0] + kernel_l + output_padding[0]
+        out_l = (
+            (in_l - 1) * stride[0]
+            - 2 * padding[0]
+            + dilation[0] * (kernel_l - 1)
+            + output_padding[0]
+            + 1
+        )
 
         if in_ch != in_channels:
             raise ShapeError(f"input channels mismatch: {in_ch} != {in_channels}.")
 
         if (_output_size := out_channels * out_l) != dest.num_in:
             raise ShapeError(f"Output size mismatch: {_output_size} != {dest.num_in}.")
 
         comm = ConvTranspose1dForward(
             (in_l,), (out_l,), _kernel, stride, padding, output_padding
         )
 
-        self.comm = comm
+        self._set_comm(comm)
 
 
 class ConvTranspose2dSyn(FullConnectedSyn):
     _spatial_ndim: ClassVar[int] = 2
 
     def __init__(
         self,
         source: Union[NeuDyn, InputProj],
         dest: Neuron,
         kernel: np.ndarray,
         stride: Tuple[int, int],
         padding: Tuple[int, int],
+        dilation: Tuple[int, int],
         output_padding: Tuple[int, int],
         order: _KOrder4d,
         name: Optional[str] = None,
     ) -> None:
         super().__init__(source, dest, name)
 
         if kernel.ndim != self._spatial_ndim + 2:
@@ -312,16 +373,28 @@
         else:
             _kernel = kernel.copy()
 
         # O,I,H,W
         out_channels, in_channels, kernel_h, kernel_w = _kernel.shape
         # C,H,W
         in_ch, in_h, in_w = _fm_ndim2_check(source.shape_out, "CHW")
-        out_h = (in_h - 1) * stride[0] - 2 * padding[0] + kernel_h + output_padding[0]
-        out_w = (in_w - 1) * stride[1] - 2 * padding[1] + kernel_w + output_padding[1]
+        out_h = (
+            (in_h - 1) * stride[0]
+            - 2 * padding[0]
+            + dilation[0] * (kernel_h - 1)
+            + output_padding[0]
+            + 1
+        )
+        out_w = (
+            (in_w - 1) * stride[1]
+            - 2 * padding[1]
+            + dilation[1] * (kernel_w - 1)
+            + output_padding[1]
+            + 1
+        )
 
         if in_ch != in_channels:
             raise ShapeError(f"input channels mismatch: {in_ch} != {in_channels}.")
 
         if (_output_size := out_channels * out_h * out_w) != dest.num_in:
             raise ShapeError(f"Output size mismatch: {_output_size} != {dest.num_in}.")
```

### Comparing `paibox-1.0.0rc1/paibox/synapses/conv_utils.py` & `paibox-1.1.0a1/paibox/components/synapses/conv_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,21 @@
 from functools import partial
 from itertools import repeat
-from typing import Any, Iterable, Literal, Tuple, TypeVar, Union
+from typing import Any, Iterable
 
 import numpy as np
 from numpy.typing import NDArray
 
 from paibox.exceptions import ShapeError
-from paibox.types import SynOutType, WeightType
+from paibox.types import SpikeType, SynOutType, WeightType
 
-T = TypeVar("T")
+from .conv_types import Size1Type, Size2Type, Size3Type, SizeAnyType, _Order2d, _Order3d
 
-_TupleAnyType = Union[T, Tuple[T, ...]]
-_Tuple1Type = Union[T, Tuple[T]]
-_Tuple2Type = Union[T, Tuple[T, T]]
-_Tuple3Type = Union[T, Tuple[T, T, T]]
 
-_SizeAnyType = _TupleAnyType[int]
-_Size1Type = _Tuple1Type[int]
-_Size2Type = _Tuple2Type[int]
-_Size3Type = _Tuple3Type[int]
-
-SizeAnyType = Tuple[int, ...]
-Size1Type = Tuple[int]
-Size2Type = Tuple[int, int]
-Size3Type = Tuple[int, int, int]
-
-_Order2d = Literal["CL", "LC"]  # Feature map order in 2d
-_Order3d = Literal["CHW", "HWC"]  # Feature map order in 3d
-_KOrder3d = Literal["OIL", "IOL"]  # Kernel order in 3d
-_KOrder4d = Literal["OIHW", "IOHW"]  # Kernel order in 4d
-
-
-def _ntuple(x, n: int) -> Tuple[Any, ...]:
+def _ntuple(x, n: int):
     if isinstance(x, Iterable):
         return tuple(x)
 
     return tuple(repeat(x, n))
 
 
 _single = partial(_ntuple, n=1)
@@ -95,17 +75,23 @@
             # [0] -> o_ch, [1] -> i_ch
             zeros_image[
                 i * stride[0] + ch_idx[1] * il : i * stride[0] + ch_idx[1] * il + kl,
                 ch_idx[0],
                 i,
             ] = kernel[ch_idx[0], ch_idx[1], :]
 
-        t = zeros_image[:, :, i].T
+        # if fm_order == "CL":
+        # (cin*il, cout) -> (cout, cin*il)
+        temp = zeros_image[:, :, i].T
+        # else:
+        #     # (cin*il, cout) -> (cout, il, cin)
+        #     temp = zeros_image[:, :, i].reshape(cin, il, cout).transpose()
+
         for o_ch in range(cout):
-            w_unrolled_np[:, i + o_ch * ol] = t[o_ch].ravel()
+            w_unrolled_np[:, i + o_ch * ol] = temp[o_ch].ravel()
 
     # Remove the part of the padding in the w_unrolled_no_padding
     # That is, remove useless weight in the w_unrolled_no_padding
     nil = in_shape[0]
     w_unrolled = np.zeros((cin * nil, cout * ol), dtype=kernel.dtype)
     for i in range(cin):
         w_unrolled[i * nil : i * nil + nil, :] = w_unrolled_np[
@@ -153,14 +139,22 @@
                 ] = kernel[ch_idx[0], ch_idx[1], :, :]
 
             t = (
                 zeros_image[:, :, i * ow + j]
                 .reshape(cin * ih, cout, iw)
                 .transpose(1, 0, 2)
             )
+            # else:
+            #     # (cin*ih, cout, iw) -> (cout, cin, ih, iw)
+            #     temp = (
+            #         zeros_image[:, :, i * ow + j]
+            #         .reshape(cin, ih, cout, iw)
+            #         .transpose(2, 1, 3, 0)
+            #     )
+
             for o_ch in range(cout):
                 w_unrolled_np[:, i * ow + j + o_ch * out_size] = t[o_ch].ravel()
 
     # Remove the part of the padding in the w_unrolled_no_padding
     # That is, remove useless weight in the w_unrolled_no_padding
     nih, niw = in_shape
     nin_size = nih * niw
@@ -178,21 +172,109 @@
                     :,
                 ]
             )
 
     return w_unrolled
 
 
+def _pool2d_kernel_unroll(
+    channels: int,
+    in_shape: Size2Type,
+    out_shape: Size2Type,
+    ksize: Size2Type,
+    stride: Size2Type,
+    # padding: Size2Type,
+    # fm_order: str,
+) -> WeightType:
+    kh, kw = ksize
+    ih, iw = in_shape
+    oh, ow = out_shape
+    in_size = ih * iw
+    out_size = oh * ow
+
+    w_unrolled = np.zeros((channels * in_size, channels * out_size), dtype=np.bool_)
+
+    for i in range(oh):
+        for j in range(ow):
+            zeros_image = np.zeros((channels * ih, iw * channels), dtype=np.bool_)
+            for i_ch in range(channels):
+                zeros_image[
+                    (i * stride[0] + i_ch * ih) : (i * stride[0] + i_ch * ih) + kh,
+                    (j * stride[1] + i_ch * iw) : (j * stride[1] + i_ch * iw) + kw,
+                ] = 1
+
+            temp = zeros_image.reshape((channels * ih, channels, iw)).transpose(1, 0, 2)
+
+            for o_ch in range(channels):
+                w_unrolled[:, i * ow + j + o_ch * oh * ow] = temp[o_ch].ravel()
+
+    return w_unrolled
+
+
+def _func_pool2d(
+    x_chw: SpikeType,
+    out_shape: Size2Type,
+    ksize: Size2Type,
+    stride: Size2Type,
+    padding: Size2Type,
+    type: str,
+) -> SpikeType:
+    xcin, xh, xw = x_chw.shape
+    kh, kw = ksize
+    oh, ow = out_shape
+    cout = xcin
+
+    assert (xh + padding[0] * 2 - kh) // stride[0] + 1 == oh
+    assert (xw + padding[1] * 2 - kw) // stride[1] + 1 == ow
+
+    out = np.zeros((cout, oh, ow), dtype=np.int32)
+    x_padded = np.pad(
+        x_chw,
+        ((0, 0), (padding[0], padding[0]), (padding[1], padding[1])),
+        mode="constant",
+    )
+
+    for c in range(cout):
+        for i in range(oh):
+            for j in range(ow):
+                if type == "avg":
+                    out[c, i, j] = np.sum(
+                        x_padded[
+                            c,
+                            stride[0] * i : stride[0] * i + kh,
+                            stride[1] * j : stride[1] * j + kw,
+                        ]
+                    )
+                else:
+                    out[c, i, j] = np.max(
+                        x_padded[
+                            c,
+                            stride[0] * i : stride[0] * i + kh,
+                            stride[1] * j : stride[1] * j + kw,
+                        ]
+                    )
+
+    if type == "avg":
+        thres = kh * kw // 2 + 1
+        return out >= thres
+    else:
+        return out.astype(np.bool_)
+
+
 def _conv1d_faster(
     x_cl: NDArray[Any],
     out_shape: Size1Type,
     kernel: WeightType,
     stride: Size1Type,
     padding: Size1Type,
 ) -> SynOutType:
+    """Faster 1d convolution.
+
+    XXX: The case where the input feature map is in 'LC' order is not considered for the time being.
+    """
     xc, xl = x_cl.shape
     # (O, I, L)
     cout, cin, kl = kernel.shape
 
     x_padded = np.pad(x_cl, ((0, 0), (padding[0], padding[0])), mode="constant")
 
     # kernel: (cout, cin, kl) -> (cout, cin*kl)
@@ -211,15 +293,20 @@
 
 def _conv2d_faster(
     x_chw: NDArray[Any],
     out_shape: Size2Type,
     kernel: WeightType,
     stride: Size2Type,
     padding: Size2Type,
+    # fm_order: str,
 ) -> SynOutType:
+    """Faster 2d convolution.
+
+    XXX: The case where the input feature map is in 'HWC' order is not considered for the time being.
+    """
     xc, xh, xw = x_chw.shape
     # (O, I, H, W)
     cout, cin, kh, kw = kernel.shape
 
     x_padded = np.pad(
         x_chw,
         ((0, 0), (padding[0], padding[0]), (padding[1], padding[1])),
```

### Comparing `paibox-1.0.0rc1/paibox/synapses/synapses.py` & `paibox-1.1.0a1/paibox/components/synapses/synapses.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,34 @@
-import warnings
+import sys
 from typing import Optional, Union
 
 import numpy as np
 
 from paibox.base import NeuDyn
-from paibox.neuron import Neuron
-from paibox.projection import InputProj
+from paibox.exceptions import PAIBoxDeprecationWarning
 from paibox.types import DataArrayType
 
+from ..neuron import Neuron
+from ..projection import InputProj
 from .base import (
     Conv1dSyn,
     Conv2dSyn,
     ConvTranspose1dSyn,
     ConvTranspose2dSyn,
     FullConnSyn,
 )
-from .conv_utils import _KOrder3d, _KOrder4d, _pair, _single, _Size1Type, _Size2Type
+from .conv_types import _KOrder3d, _KOrder4d, _Size1Type, _Size2Type
+from .conv_utils import _pair, _single
 from .transforms import GeneralConnType as GConnType
 
+if sys.version_info >= (3, 13):
+    from warnings import deprecated
+else:
+    from typing_extensions import deprecated
+
 __all__ = ["FullConn", "Conv1d", "Conv2d", "ConvTranspose1d", "ConvTranspose2d"]
 
 
 class FullConn(FullConnSyn):
     def __init__(
         self,
         source: Union[NeuDyn, InputProj],
@@ -39,29 +46,28 @@
             - weights: weights of the synapses. It can be a scalar or `np.ndarray`.
             - conn_type: the type of connection.
             - name: name of the full-connected synapses. Optional.
         """
         super().__init__(source, dest, weights, conn_type, name)
 
 
+@deprecated(
+    "'NoDecay' will be removed in a future version. Use 'FullConn' instead.",
+    category=PAIBoxDeprecationWarning,
+)
 class NoDecay(FullConn):
     def __init__(
         self,
         source: Union[NeuDyn, InputProj],
         dest: NeuDyn,
         weights: DataArrayType = 1,
         *,
         conn_type: GConnType = GConnType.MatConn,
         name: Optional[str] = None,
     ) -> None:
-        warnings.warn(
-            "'NoDecay' class will be deprecated in future versions. Use 'FullConn' instead.",
-            DeprecationWarning,
-        )
-
         super().__init__(source, dest, weights, conn_type=conn_type, name=name)
 
 
 class Conv1d(Conv1dSyn):
     def __init__(
         self,
         source: Union[Neuron, InputProj],
@@ -88,15 +94,22 @@
 
         NOTE: See https://pytorch.org/docs/stable/generated/torch.nn.Conv1d.html#torch.nn.Conv1d for details.
         """
         if kernel_order not in ("OIL", "IOL"):
             raise ValueError(f"kernel order must be 'OIL' or 'IOL'.")
 
         super().__init__(
-            source, dest, kernel, _single(stride), _single(padding), kernel_order, name
+            source,
+            dest,
+            kernel,
+            _single(stride),
+            _single(padding),
+            _single(1),
+            kernel_order,
+            name,
         )
 
 
 class Conv2d(Conv2dSyn):
     def __init__(
         self,
         source: Union[Neuron, InputProj],
@@ -123,15 +136,22 @@
 
         NOTE: See https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html#torch.nn.Conv2d for details.
         """
         if kernel_order not in ("OIHW", "IOHW"):
             raise ValueError(f"kernel order must be 'OIHW' or 'IOHW'.")
 
         super().__init__(
-            source, dest, kernel, _pair(stride), _pair(padding), kernel_order, name
+            source,
+            dest,
+            kernel,
+            _pair(stride),
+            _pair(padding),
+            _pair(1),
+            kernel_order,
+            name,
         )
 
 
 class ConvTranspose1d(ConvTranspose1dSyn):
     def __init__(
         self,
         source: Union[Neuron, InputProj],
@@ -168,14 +188,15 @@
         super().__init__(
             source,
             dest,
             kernel,
             _single(stride),
             _single(padding),
             _single(output_padding),
+            _single(1),
             kernel_order,
             name,
         )
 
 
 class ConvTranspose2d(ConvTranspose2dSyn):
     def __init__(
@@ -217,10 +238,11 @@
         super().__init__(
             source,
             dest,
             kernel,
             _pair(stride),
             _pair(padding),
             _pair(output_padding),
+            _pair(1),
             kernel_order,
             name,
         )
```

### Comparing `paibox-1.0.0rc1/paibox/synapses/transforms.py` & `paibox-1.1.0a1/paibox/components/synapses/transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import warnings
 from enum import Enum, auto, unique
+from typing import Literal
 
 import numpy as np
 from paicorelib import WeightPrecision as WP
 
 from paibox.exceptions import AutoOptimizationWarning, ShapeError
-from paibox.types import DataArrayType, IntScalarType, SynOutType, WeightType
+from paibox.types import DataArrayType, IntScalarType, SpikeType, SynOutType, WeightType
 from paibox.utils import is_shape
 
+from .conv_types import Size1Type, Size2Type
 from .conv_utils import (
-    Size1Type,
-    Size2Type,
     _conv1d_faster,
     _conv1d_unroll,
     _conv2d_faster,
     _conv2d_unroll,
     _convtranspose1d_faster,
     _convtranspose1d_unroll,
     _convtranspose2d_faster,
     _convtranspose2d_unroll,
+    _func_pool2d,
+    _pool2d_kernel_unroll,
 )
 
 __all__ = [
-    "GeneralConnType",
     "OneToOne",
     "AllToAll",
     "Identity",
     "MaskedLinear",
-    "Conv1dForward",
     "Conv2dForward",
     "ConvTranspose1dForward",
     "ConvTranspose2dForward",
 ]
 
 
 MAX_INT1 = np.int8(1)
@@ -187,22 +187,22 @@
 
         # The ndim of weights = 0 or 1.
         if self.weights.ndim not in (0, 1):
             raise ShapeError(
                 f"the ndim of weights must be 0 or 1, but got {self.weights.ndim}."
             )
 
-    def __call__(self, x: np.ndarray, *args, **kwargs) -> SynOutType:
+    def __call__(self, x: SpikeType, *args, **kwargs) -> SynOutType:
         # (N,) * (N,) -> (N,)
         return x * self.weights.astype(np.int32)
 
     @property
     def connectivity(self):
         return (
-            (self.weights * np.eye(self.num, dtype=np.bool_))
+            (self.weights * np.identity(self.num, dtype=np.bool_))
             if self.weights.ndim == 0
             else np.diag(self.weights)
         )
 
 
 class Identity(OneToOne):
     def __init__(self, num: int, scaling_factor: IntScalarType = 1) -> None:
@@ -235,15 +235,15 @@
         super().__init__(weights)
 
         if self.weights.ndim not in (0, 2):
             raise ShapeError(
                 f"the ndim of weights must be 0 or 2, but got {self.weights.ndim}."
             )
 
-    def __call__(self, x: np.ndarray, *args, **kwargs) -> SynOutType:
+    def __call__(self, x: SpikeType, *args, **kwargs) -> SynOutType:
         """
         NOTE:
             - When weights is a scalar, the output is a scalar (sum * w) & repeated     \
                 `conn_size[1]` times.
             - When weights is a matrix, the output is the dot product of `x` & weights.
         """
         if self.weights.ndim == 0:
@@ -268,15 +268,15 @@
 class MaskedLinear(Transform):
     def __init__(self, conn_size: Size2Type, weights: np.ndarray) -> None:
         if not is_shape(weights, conn_size):
             raise ShapeError(f"expected shape is {conn_size}, but got {weights.shape}.")
 
         super().__init__(weights)
 
-    def __call__(self, x: np.ndarray, *args, **kwargs) -> SynOutType:
+    def __call__(self, x: SpikeType, *args, **kwargs) -> SynOutType:
         # (N,) @ (N, M) -> (M,)
         return x @ self.weights.astype(np.int32)
 
     @property
     def connectivity(self):
         return self.weights
 
@@ -295,15 +295,15 @@
         self.out_shape = out_shape
         self.stride = stride
         self.padding = padding
         # self.fm_order = fm_order
 
         super().__init__(kernel)
 
-    def __call__(self, x: np.ndarray, *args, **kwargs) -> SynOutType:
+    def __call__(self, x: SpikeType, *args, **kwargs) -> SynOutType:
         cin = self.weights.shape[1]
 
         # if self.fm_order == "LC":
         #     # (N,) -> (L, C) -> (C, L)
         #     _x = x.reshape(self.in_shape + (cin,)).T
         # else:
         _x = x.reshape((cin,) + self.in_shape)
@@ -333,15 +333,15 @@
         self.out_shape = out_shape
         self.stride = stride
         self.padding = padding
         # self.fm_order = fm_order
 
         super().__init__(kernel)
 
-    def __call__(self, x: np.ndarray, *args, **kwargs) -> SynOutType:
+    def __call__(self, x: SpikeType, *args, **kwargs) -> SynOutType:
         cin = self.weights.shape[1]
 
         # if self.fm_order == "HWC":
         #     # (N,) -> (H, W, C) -> (C, H, W)
         #     _x = x.reshape(self.in_shape + (cin,)).transpose(2, 0, 1)
         # else:
         _x = x.reshape((cin,) + self.in_shape)
@@ -451,7 +451,53 @@
             self.in_shape,
             self.out_shape,
             self.weights,
             self.stride,
             self.padding,
             self.output_padding,
         )
+
+
+class _Pool2dForward(Transform):
+    # DO NOT use in the `FullConnectedSyn`
+    def __init__(
+        self,
+        channels: int,
+        in_shape: Size2Type,
+        out_shape: Size2Type,
+        kernel_size: Size2Type,
+        stride: Size2Type,
+        padding: Size2Type,
+        # fm_order: _Order3d,
+        pool_type: Literal["avg", "max"],
+    ) -> None:
+        self.channels = channels
+        self.in_shape = in_shape
+        self.out_shape = out_shape
+        self.ksize = kernel_size
+        self.stride = stride
+        self.padding = padding
+        # self.fm_order = fm_order
+        self.pool_type = pool_type
+
+        super().__init__(np.asarray(1, dtype=np.int8))
+
+    def __call__(self, x: SpikeType, *args, **kwargs) -> SpikeType:
+        # if self.fm_order == "HWC":
+        #     # (N,) -> (H, W, C) -> (C, H, W)
+        #     _x = x.reshape(self.in_shape + (self.channels,)).transpose(2, 0, 1)
+        # else:
+        _x = x.reshape((self.channels,) + self.in_shape)
+
+        return _func_pool2d(
+            _x, self.out_shape, self.ksize, self.stride, self.padding, self.pool_type
+        )
+
+    @property
+    def connectivity(self):
+        return _pool2d_kernel_unroll(
+            self.channels,
+            self.in_shape,
+            self.out_shape,
+            self.ksize,
+            self.stride,
+        )
```

### Comparing `paibox-1.0.0rc1/paibox/types.py` & `paibox-1.1.0a1/paibox/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from typing import (
     AbstractSet,
     Any,
-    Generic,
     Iterable,
     Iterator,
     List,
     MutableSet,
     NoReturn,
     Optional,
     Tuple,
     TypeVar,
     Union,
 )
 
 import numpy as np
 from numpy.typing import NDArray
+from typing_extensions import TypeAlias
 
 Shape = TypeVar("Shape", int, Tuple[int, ...], List[int])
 ArrayType = TypeVar("ArrayType", List[int], Tuple[int, ...], np.ndarray)
 Scalar = TypeVar("Scalar", int, float, np.generic)
 IntScalarType = TypeVar("IntScalarType", int, np.bool_, np.integer)
 DataType = TypeVar("DataType", int, np.bool_, np.integer, np.ndarray)
 DataArrayType = TypeVar(
     "DataArrayType", int, np.bool_, np.integer, List[int], Tuple[int, ...], np.ndarray
 )
-SpikeType = NDArray[np.bool_]
-SynOutType = NDArray[np.int32]
-VoltageType = NDArray[np.int32]
-WeightType = NDArray[Union[np.bool_, np.int8]]
+SpikeType: TypeAlias = NDArray[np.bool_]
+SynOutType: TypeAlias = NDArray[np.int32]
+VoltageType: TypeAlias = NDArray[np.int32]
+WeightType: TypeAlias = NDArray[Union[np.bool_, np.int8]]
 
 _T = TypeVar("_T")
 
 
-class FrozenOrderedSet(AbstractSet, Generic[_T]):
+class FrozenOrderedSet(AbstractSet[_T]):
     """A set that preserves insertion order and is hashable."""
 
     def __init__(self, data: Optional[Iterable[Any]] = None) -> None:
         if data is None:
             data = []
 
         self.data = dict.fromkeys(data)
```

### Comparing `paibox-1.0.0rc1/paibox/utils.py` & `paibox-1.1.0a1/paibox/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,14 +31,26 @@
     seen = set()
     for item in obj:
         seen.add(item)
 
     return len(seen)
 
 
+def merge_unique_ordered(list1: List[Any], list2: List[Any]) -> List[Any]:
+    seen = set()
+    result = []
+
+    for item in list1 + list2:
+        if item not in seen:
+            seen.add(item)
+            result.append(item)
+
+    return result
+
+
 def check_attr_same(obj: Sequence[Any], attr: str) -> bool:
     return all(getattr(obj[0], attr) == getattr(item, attr) for item in obj)
 
 
 def check_elem_same(obj: Any) -> bool:
     if hasattr(obj, "__iter__") or hasattr(obj, "__contains__"):
         return len(set(obj)) == 1
@@ -64,25 +76,28 @@
         a = 1
         for b in shape:
             a *= b
 
         return a
 
 
-def as_shape(shape, min_dim: int = 0) -> Tuple[int, ...]:
-    """Convert a shape to a tuple, like (1,), (10,), or (10, 20)"""
-    if is_integer(shape):
-        _shape = (shape,)
-    elif is_iterable(shape):
-        _shape = tuple(shape)
+def as_shape(x, min_dim: int = 0) -> Tuple[int, ...]:
+    """Return a tuple if `x` is iterable or `(x,)` if `x` is integer."""
+    if is_integer(x):
+        _shape = (x,)
+    elif is_iterable(x):
+        if isinstance(x, np.ndarray):
+            _shape = tuple(x.astype(int))
+        else:
+            _shape = tuple(x)
     else:
-        raise ValueError(f"cannot make a shape for {shape}.")
+        raise ValueError(f"{x} cannot be safely converted to a shape.")
 
     if len(_shape) < min_dim:
-        _shape = tuple([1] * (min_dim - len(_shape))) + _shape
+        _shape = (1,) * (min_dim - len(_shape)) + _shape
 
     return _shape
 
 
 def is_shape(x, shape: Shape) -> bool:
     if not is_array_like(x):
         raise TypeError(f"only support an array-like type: {x}.")
```

### Comparing `paibox-1.0.0rc1/pyproject.toml` & `paibox-1.1.0a1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "paibox"
-version = "1.0.0rc1"
-description = "Toolchain of PAICORE 2.0."
+version = "1.1.0a1"
+description = "Toolchain of PAICORE 2.0"
 authors = ["Ziru Pan <zrpan@stu.pku.edu.cn>"]
 maintainers = [
     "Hongtu Xia <hongtux@pku.edu.cn>",
     "Siyuan Gao <siyuan-gao@outlook.com>",
     "Zhaoyang Hao <hzyang2218@gmail.com>",
     "Ziru Pan <zrpan@stu.pku.edu.cn>",
 ]
@@ -28,31 +28,38 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries",
 ]
 packages = [{ include = "paibox" }]
 
 # Includes the document
-include = ["docs", "CHANGELOG.md"]
-# Excludes the experimental code
-exclude = ["paibox/experimental"]
+include = ["docs/Guide-of-PAIBox.md", "CHANGELOG.md"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^2.0"
 numpy = "^1.24.0"
-paicorelib = "^0.0.13"
+paicorelib = "^1.1.1"
 
 [tool.poetry.group.test]
 optional = true
 
+[tool.poetry.group.dev]
+optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = { version = "^7.4.0", python = "^3.8" }
+pytest = { version = "^8.0.0", python = "^3.8" }
+pytest-md = "^0.2.0"
 torch = { version = "^2.2.1+cpu", optional = true, source = "torch-cpu" }
+paicorelib = {git = "https://github.com/PAICookers/PAIlib.git", rev = "dev"}
+orjson = "^3.10.1"
+
+
+[tool.poetry.group.dev.dependencies]
+orjson = "^3.10.1"
 
 
 [tool.pytest.ini_options]
 minversion = "7.0.0"
 testpaths = ["tests"]
```

### Comparing `paibox-1.0.0rc1/PKG-INFO` & `paibox-1.1.0a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: paibox
-Version: 1.0.0rc1
-Summary: Toolchain of PAICORE 2.0.
+Version: 1.1.0a1
+Summary: Toolchain of PAICORE 2.0
 Home-page: https://github.com/PAICookers/PAIBox
 License: GPL-3.0-or-later
 Keywords: PAICORE 2.0,PAIBox,SNN,Toolchain
 Author: Ziru Pan
 Author-email: zrpan@stu.pku.edu.cn
 Maintainer: Hongtu Xia
 Maintainer-email: hongtux@pku.edu.cn
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: numpy (>=1.24.0,<2.0.0)
-Requires-Dist: paicorelib (>=0.0.13,<0.0.14)
+Requires-Dist: paicorelib (>=1.1.1,<2.0.0)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Project-URL: Documentation, https://github.com/PAICookers/PAIBox#readme
 Project-URL: Repository, https://github.com/PAICookers/PAIBox
 Description-Content-Type: text/markdown
 
 <div align="center">
 
@@ -36,26 +36,24 @@
 
 </div>
 
 <p align="center">
     <a href="https://github.com/PAICookers/PAIBox/blob/master/pyproject.toml">
         <img src="https://img.shields.io/pypi/pyversions/paibox">
     </a>
-    <a href="https://github.com/PAICookers/PAIBox/releases/tag/v1.0.0rc1">
-        <img src="https://img.shields.io/github/v/release/PAICookers/PAIBox?include_prereleases&color=orange">
+    <a href="https://github.com/PAICookers/PAIBox/releases/tag/v1.1.0a1">
+        <img src="https://img.shields.io/github/v/release/PAICookers/PAIBox&color=orange">
     </a>
     <a href="https://www.codefactor.io/repository/github/PAICookers/PAIBox">
       <img src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIBox/master?color=red">
     </a>
     <a href="https://results.pre-commit.ci/latest/github/PAICookers/PAIBox/master">
 	   <img src="https://results.pre-commit.ci/badge/github/PAICookers/PAIBox/master.svg" alt="pre-commit.ci status">
     </a>
 </p>
 
-PAIBox使用指南：[Guide-of-PAIBox](docs/Guide-of-PAIBox.md)
+👉 用户使用指南：[Guide-of-PAIBox](docs/Guide-of-PAIBox.md)
 
 高效编写测试项目指南：[Guide-of-Test](docs/Guide-of-Test.md)
 
-TODO：[TODO List](./TODO.md)
-
 [Changelog](./CHANGELOG.md)
```

#### html2text {}

```diff
@@ -1,27 +1,26 @@
-Metadata-Version: 2.1 Name: paibox Version: 1.0.0rc1 Summary: Toolchain of
-PAICORE 2.0. Home-page: https://github.com/PAICookers/PAIBox License: GPL-3.0-
+Metadata-Version: 2.1 Name: paibox Version: 1.1.0a1 Summary: Toolchain of
+PAICORE 2.0 Home-page: https://github.com/PAICookers/PAIBox License: GPL-3.0-
 or-later Keywords: PAICORE 2.0,PAIBox,SNN,Toolchain Author: Ziru Pan Author-
 email: zrpan@stu.pku.edu.cn Maintainer: Hongtu Xia Maintainer-email:
 hongtux@pku.edu.cn Requires-Python: >=3.8,<4.0 Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development :: Build Tools Classifier: Topic :: Software Development ::
 Libraries Requires-Dist: numpy (>=1.24.0,<2.0.0) Requires-Dist: paicorelib
-(>=0.0.13,<0.0.14) Requires-Dist: pydantic (>=2.0,<3.0) Project-URL:
+(>=1.1.1,<2.0.0) Requires-Dist: pydantic (>=2.0,<3.0) Project-URL:
 Documentation, https://github.com/PAICookers/PAIBox#readme Project-URL:
 Repository, https://github.com/PAICookers/PAIBox Description-Content-Type:
 text/markdown
                                    # PAIBox
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_p_a_i_b_o_x_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
-    _v_/_r_e_l_e_a_s_e_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_?_i_n_c_l_u_d_e___p_r_e_r_e_l_e_a_s_e_s_&_c_o_l_o_r_=_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_f_a_c_t_o_r_/_g_r_a_d_e_/_g_i_t_h_u_b_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_/_m_a_s_t_e_r_?_c_o_l_o_r_=_r_e_d_]_[_p_r_e_-
-                               _c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]
-PAIBoxä½¿ç¨æåï¼[Guide-of-PAIBox](docs/Guide-of-PAIBox.md)
-é«æç¼åæµè¯é¡¹ç®æåï¼[Guide-of-Test](docs/Guide-of-Test.md) TODOï¼
-[TODO List](./TODO.md) [Changelog](./CHANGELOG.md)
+ _v_/_r_e_l_e_a_s_e_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_&_c_o_l_o_r_=_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_f_a_c_t_o_r_/
+    _g_r_a_d_e_/_g_i_t_h_u_b_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_/_m_a_s_t_e_r_?_c_o_l_o_r_=_r_e_d_]_[_p_r_e_-_c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]
+ð ç¨æ·ä½¿ç¨æåï¼[Guide-of-PAIBox](docs/Guide-of-PAIBox.md)
+é«æç¼åæµè¯é¡¹ç®æåï¼[Guide-of-Test](docs/Guide-of-Test.md)
+[Changelog](./CHANGELOG.md)
```

