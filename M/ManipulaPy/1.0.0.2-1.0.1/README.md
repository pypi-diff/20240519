# Comparing `tmp/ManipulaPy-1.0.0.2.tar.gz` & `tmp/ManipulaPy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ManipulaPy-1.0.0.2.tar", last modified: Fri May  3 18:57:11 2024, max compression
+gzip compressed data, was "ManipulaPy-1.0.1.tar", last modified: Sun May 19 20:06:42 2024, max compression
```

## Comparing `ManipulaPy-1.0.0.2.tar` & `ManipulaPy-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 abo       (1000) abo       (1000)        0 2024-05-03 18:57:11.239327 ManipulaPy-1.0.0.2/
--rw-rw-r--   0 abo       (1000) abo       (1000)     1077 2024-04-28 20:45:53.000000 ManipulaPy-1.0.0.2/LICENSE.md
-drwxrwxr-x   0 abo       (1000) abo       (1000)        0 2024-05-03 18:57:11.239327 ManipulaPy-1.0.0.2/ManipulaPy/
--rw-rw-r--   0 abo       (1000) abo       (1000)      320 2024-05-03 18:52:30.000000 ManipulaPy-1.0.0.2/ManipulaPy/__init__.py
--rw-rw-r--   0 abo       (1000) abo       (1000)     6801 2024-04-28 20:45:53.000000 ManipulaPy-1.0.0.2/ManipulaPy/dynamics.py
--rw-rw-r--   0 abo       (1000) abo       (1000)     8673 2024-04-28 20:45:53.000000 ManipulaPy-1.0.0.2/ManipulaPy/kinematics.py
--rw-rw-r--   0 abo       (1000) abo       (1000)    11576 2024-04-28 20:45:53.000000 ManipulaPy-1.0.0.2/ManipulaPy/path_planning.py
--rw-rw-r--   0 abo       (1000) abo       (1000)     9557 2024-04-28 20:45:53.000000 ManipulaPy-1.0.0.2/ManipulaPy/singularity.py
--rw-rw-r--   0 abo       (1000) abo       (1000)     2001 2024-04-28 20:45:53.000000 ManipulaPy-1.0.0.2/ManipulaPy/transformations.py
--rw-rw-r--   0 abo       (1000) abo       (1000)    10404 2024-04-28 20:45:53.000000 ManipulaPy-1.0.0.2/ManipulaPy/urdf_processor.py
--rw-rw-r--   0 abo       (1000) abo       (1000)     9433 2024-04-28 20:45:53.000000 ManipulaPy-1.0.0.2/ManipulaPy/utils.py
-drwxrwxr-x   0 abo       (1000) abo       (1000)        0 2024-05-03 18:57:11.239327 ManipulaPy-1.0.0.2/ManipulaPy.egg-info/
--rw-r--r--   0 abo       (1000) abo       (1000)     1538 2024-05-03 18:57:11.000000 ManipulaPy-1.0.0.2/ManipulaPy.egg-info/PKG-INFO
--rw-rw-r--   0 abo       (1000) abo       (1000)      402 2024-05-03 18:57:11.000000 ManipulaPy-1.0.0.2/ManipulaPy.egg-info/SOURCES.txt
--rw-rw-r--   0 abo       (1000) abo       (1000)        1 2024-05-03 18:57:11.000000 ManipulaPy-1.0.0.2/ManipulaPy.egg-info/dependency_links.txt
--rw-rw-r--   0 abo       (1000) abo       (1000)       28 2024-05-03 18:57:11.000000 ManipulaPy-1.0.0.2/ManipulaPy.egg-info/requires.txt
--rw-rw-r--   0 abo       (1000) abo       (1000)       11 2024-05-03 18:57:11.000000 ManipulaPy-1.0.0.2/ManipulaPy.egg-info/top_level.txt
--rw-r--r--   0 abo       (1000) abo       (1000)     1538 2024-05-03 18:57:11.239327 ManipulaPy-1.0.0.2/PKG-INFO
--rw-rw-r--   0 abo       (1000) abo       (1000)      985 2024-04-28 20:45:53.000000 ManipulaPy-1.0.0.2/README.md
--rw-rw-r--   0 abo       (1000) abo       (1000)       38 2024-05-03 18:57:11.239327 ManipulaPy-1.0.0.2/setup.cfg
--rw-rw-r--   0 abo       (1000) abo       (1000)      923 2024-05-03 18:56:38.000000 ManipulaPy-1.0.0.2/setup.py
+drwxrwxr-x   0 abo       (1000) abo       (1000)        0 2024-05-19 20:06:42.754591 ManipulaPy-1.0.1/
+-rw-rw-r--   0 abo       (1000) abo       (1000)     1077 2024-04-28 20:45:53.000000 ManipulaPy-1.0.1/LICENSE.md
+drwxrwxr-x   0 abo       (1000) abo       (1000)        0 2024-05-19 20:06:42.750591 ManipulaPy-1.0.1/ManipulaPy/
+-rw-rw-r--   0 abo       (1000) abo       (1000)      662 2024-05-19 20:05:33.000000 ManipulaPy-1.0.1/ManipulaPy/__init__.py
+-rw-rw-r--   0 abo       (1000) abo       (1000)    11181 2024-05-19 19:45:19.000000 ManipulaPy-1.0.1/ManipulaPy/controller.py
+-rw-rw-r--   0 abo       (1000) abo       (1000)     6801 2024-04-28 20:45:53.000000 ManipulaPy-1.0.1/ManipulaPy/dynamics.py
+-rw-rw-r--   0 abo       (1000) abo       (1000)     8673 2024-04-28 20:45:53.000000 ManipulaPy-1.0.1/ManipulaPy/kinematics.py
+-rw-rw-r--   0 abo       (1000) abo       (1000)    24569 2024-05-19 17:02:36.000000 ManipulaPy-1.0.1/ManipulaPy/path_planning.py
+-rw-rw-r--   0 abo       (1000) abo       (1000)     6318 2024-05-18 12:59:33.000000 ManipulaPy-1.0.1/ManipulaPy/singularity.py
+-rw-rw-r--   0 abo       (1000) abo       (1000)     2001 2024-04-28 20:45:53.000000 ManipulaPy-1.0.1/ManipulaPy/transformations.py
+-rw-rw-r--   0 abo       (1000) abo       (1000)    11684 2024-05-18 14:06:37.000000 ManipulaPy-1.0.1/ManipulaPy/urdf_processor.py
+-rw-rw-r--   0 abo       (1000) abo       (1000)    10160 2024-05-19 09:23:53.000000 ManipulaPy-1.0.1/ManipulaPy/utils.py
+drwxrwxr-x   0 abo       (1000) abo       (1000)        0 2024-05-19 20:06:42.750591 ManipulaPy-1.0.1/ManipulaPy.egg-info/
+-rw-r--r--   0 abo       (1000) abo       (1000)     6062 2024-05-19 20:06:42.000000 ManipulaPy-1.0.1/ManipulaPy.egg-info/PKG-INFO
+-rw-rw-r--   0 abo       (1000) abo       (1000)      427 2024-05-19 20:06:42.000000 ManipulaPy-1.0.1/ManipulaPy.egg-info/SOURCES.txt
+-rw-rw-r--   0 abo       (1000) abo       (1000)        1 2024-05-19 20:06:42.000000 ManipulaPy-1.0.1/ManipulaPy.egg-info/dependency_links.txt
+-rw-rw-r--   0 abo       (1000) abo       (1000)       72 2024-05-19 20:06:42.000000 ManipulaPy-1.0.1/ManipulaPy.egg-info/requires.txt
+-rw-rw-r--   0 abo       (1000) abo       (1000)       11 2024-05-19 20:06:42.000000 ManipulaPy-1.0.1/ManipulaPy.egg-info/top_level.txt
+-rw-r--r--   0 abo       (1000) abo       (1000)     6062 2024-05-19 20:06:42.750591 ManipulaPy-1.0.1/PKG-INFO
+-rw-rw-r--   0 abo       (1000) abo       (1000)     5452 2024-05-19 19:58:54.000000 ManipulaPy-1.0.1/README.md
+-rw-rw-r--   0 abo       (1000) abo       (1000)       38 2024-05-19 20:06:42.754591 ManipulaPy-1.0.1/setup.cfg
+-rw-rw-r--   0 abo       (1000) abo       (1000)      842 2024-05-19 20:05:20.000000 ManipulaPy-1.0.1/setup.py
```

### Comparing `ManipulaPy-1.0.0.2/LICENSE.md` & `ManipulaPy-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ManipulaPy-1.0.0.2/ManipulaPy/dynamics.py` & `ManipulaPy-1.0.1/ManipulaPy/dynamics.py`

 * *Files identical despite different names*

### Comparing `ManipulaPy-1.0.0.2/ManipulaPy/kinematics.py` & `ManipulaPy-1.0.1/ManipulaPy/kinematics.py`

 * *Files identical despite different names*

### Comparing `ManipulaPy-1.0.0.2/ManipulaPy/transformations.py` & `ManipulaPy-1.0.1/ManipulaPy/transformations.py`

 * *Files identical despite different names*

### Comparing `ManipulaPy-1.0.0.2/ManipulaPy/urdf_processor.py` & `ManipulaPy-1.0.1/ManipulaPy/urdf_processor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
 
+
 from urchin.urdf import URDF 
 import numpy as np
 import pybullet as p
 import pybullet_data
 import time
 from .kinematics import SerialManipulator
 from .dynamics import ManipulatorDynamics
 from . import utils
-import matplotlib.pyplot as plt
-import matplotlib.pyplot as plt
-from .utils import adjoint_transform, transform_from_twist
+
+
 class URDFToSerialManipulator:
     """
     A class to convert URDF files to SerialManipulator objects and simulate them using PyBullet.
     """
 
     def __init__(self, urdf_name: str):
         """
@@ -22,18 +22,19 @@
 
         Parameters:
             urdf_name (str): The name of the URDF file.
 
         Returns:
             None
         """
-        
         self.urdf_name = urdf_name
+        self.robot = URDF.load(urdf_name)
         self.robot_data = self.load_urdf(urdf_name)
         self.serial_manipulator = self.initialize_serial_manipulator()
+        self.dynamics = self.initialize_manipulator_dynamics()
 
     @staticmethod
     def transform_to_xyz(T: np.ndarray) -> np.ndarray:
         """
         Extracts the XYZ position from a transformation matrix.
 
         Args:
@@ -71,15 +72,15 @@
         :param robot_dof: An integer representing the number of degrees of freedom of the robot.
         :return: A numpy array representing the screw list.
         """
         Slist = []
         for i in range(robot_dof):
             w_ = w[i]
             p_ = p[i]
-            v_ = np.cross(w_, -p_)
+            v_ = np.cross(-1*w_, p_)
             Slist.append([w_[0], w_[1], w_[2], v_[0], v_[1], v_[2]])
         return np.transpose(Slist)
 
     def load_urdf(self, urdf_name: str) -> dict:
         """
         Load the URDF file and extract the necessary information to create the robot model.
 
@@ -147,15 +148,29 @@
             omega_list=data["Slist"][:, :3],
             r_list=utils.extract_r_list(data["Slist"]),
             b_list=None,  # Assuming b_list is not provided in URDF data
             S_list=data["Slist"],
             B_list=data["Blist"],
             Glist=data["Glist"]
         )
-
+    def initialize_manipulator_dynamics(self):
+        """
+        Initializes the ManipulatorDynamics object using the extracted URDF data.
+        """
+        data = self.robot_data
+        # Initialize the ManipulatorDynamics object
+        self.manipulator_dynamics = ManipulatorDynamics(
+            M_list=data["M"],
+            omega_list=data["Slist"][:, :3],
+            r_list=utils.extract_r_list(data["Slist"]),
+            b_list=None,  # Assuming b_list is not provided in URDF data
+            S_list=data["Slist"],
+            B_list=data["Blist"],
+            Glist=data["Glist"]
+        )
         return self.manipulator_dynamics
     def extract_inertia_matrices(self):
         """
         Extracts the spatial inertia matrices from the URDF data.
         """
         Glist = []
         for link in self.robot.links:
@@ -166,46 +181,14 @@
                 G[:3, :3] = inertia
                 G[3:, 3:] = mass * np.eye(3)
                 Glist.append(G)
             else:
                 Glist.append(np.zeros((6, 6)))  # Add zero matrix for links without inertia
         return Glist
 
-    def visualize_robot(self, thetalist):
-        """
-        Visualize the robot using Matplotlib based on the provided joint angles.
-
-        Args:
-            thetalist (np.ndarray): The joint angles of the robot.
-        """
-        fig = plt.figure()
-        ax = fig.add_subplot(111, projection='3d')
-
-        # Starting point (base of the robot)
-        T = np.eye(4)
-        x, y, z = T[0, 3], T[1, 3], T[2, 3]
-        ax.scatter(x, y, z, color='k')  # Base point
-
-        for i in range(len(thetalist)):
-            # Compute the forward kinematics for each joint
-            T = np.dot(T, self.serial_manipulator.forward_kinematics(thetalist[:i + 1], 'space'))
-            x, y, z = T[0, 3], T[1, 3], T[2, 3]
-            ax.scatter(x, y, z, color='r')  # Joint points
-
-            # Plot the links between joints
-            if i > 0:
-                prev_x, prev_y, prev_z = prev_T[0, 3], prev_T[1, 3], prev_T[2, 3]
-                ax.plot([prev_x, x], [prev_y, y], [prev_z, z], color='b')  # Links
-
-            prev_T = T
-
-        ax.set_xlabel('X axis')
-        ax.set_ylabel('Y axis')
-        ax.set_zlabel('Z axis')
-        ax
     def simulate_robot(self):
         """
         Simulates the robot using PyBullet.
         """
         M = self.robot_data["M"]
         Slist = self.robot_data["Slist"]
         Blist = self.robot_data["Blist"]
@@ -265,7 +248,47 @@
         p.setTimeStep(timeStep)
         while p.isConnected():
             p.stepSimulation()
             time.sleep(timeStep)  # Simulation time step
         time.sleep(10*np.exp(100))
         # Disconnect from PyBullet
         p.disconnect()
+
+    def visualize_robot(self):
+        """
+        Visualizes the URDF model using matplotlib.
+        """
+        
+        self.robot.show()
+    
+
+    def visualize_trajectory(self, cfg_trajectory=None, loop_time=3.0, use_collision=False):
+        # Filter out fixed joints
+        actuated_joints = [joint for joint in self.robot.joints if joint.joint_type != 'fixed']
+        
+        if cfg_trajectory is not None:
+            if isinstance(cfg_trajectory, np.ndarray):
+                expected_columns = len(actuated_joints)
+                if cfg_trajectory.shape[1] != expected_columns:
+                    raise ValueError(f"Expected cfg_trajectory to have {expected_columns} columns, got {cfg_trajectory.shape[1]}.")
+                cfg_trajectory = {joint.name: cfg_trajectory[:, i] for i, joint in enumerate(actuated_joints) if i < cfg_trajectory.shape[1]}
+            elif isinstance(cfg_trajectory, dict):
+                if len(cfg_trajectory) != len(actuated_joints):
+                    raise ValueError(f"Expected cfg_trajectory keys to match the number of robot joints ({len(actuated_joints)}), got {len(cfg_trajectory)}.")
+            else:
+                raise TypeError("cfg_trajectory must be either a numpy array or a dictionary mapping joint names to configurations.")
+        else:
+            cfg_trajectory = {joint.name: [0, np.pi / 2] for joint in actuated_joints}
+
+        self.robot.animate(cfg_trajectory=cfg_trajectory, loop_time=loop_time, use_collision=use_collision)
+
+    def print_joint_info(self):
+        """
+        Prints the number of joints and their names.
+        """
+        joint_names = [joint.name for joint in self.robot.joints]
+        print(f"Number of joints: {len(joint_names)}")
+        for i, joint_name in enumerate(joint_names):
+            print(f"Joint {i}: {joint_name}")
+
+
+
```

### Comparing `ManipulaPy-1.0.0.2/ManipulaPy/utils.py` & `ManipulaPy-1.0.1/ManipulaPy/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,277 +9,339 @@
     
     Parameters:
         Slist (list): A list of S vectors representing the joint screws.
         
     Returns:
         np.ndarray: An array of r vectors.
     """
-    
     r_list = []
     for S in np.array(Slist).T:
         omega = S[:3]
         v = S[3:]
         if np.linalg.norm(omega) != 0:
             r = -np.cross(omega, v) / np.linalg.norm(omega)**2
             r_list.append(r)
         else:
             r_list.append([0, 0, 0])  # For prismatic joints
     return np.array(r_list)
-def NearZero(z):
-    """
-    Determines if a given number is near zero.
-
-    Parameters:
-        z (float): The number to check.
 
-    Returns:
-        bool: True if the number is near zero, False otherwise.
-    """
-    
-    return abs(z) < 1e-6
 def extract_omega_list(Slist):
     """
     Extracts the first three elements from each sublist in the given list and returns them as a numpy array.
 
     Parameters:
         Slist (list): A list of sublists.
 
     Returns:
         np.array: A numpy array containing the first three elements from each sublist.
     """
-    
     return np.array(Slist)[:, :3]
 
+def NearZero(z):
+    """
+    Determines if a given number is near zero.
+
+    Parameters:
+        z (float): The number to check.
+
+    Returns:
+        bool: True if the number is near zero, False otherwise.
+    """
+    return abs(z) < 1e-6
+
 def skew_symmetric(v):
     """
     Returns the skew symmetric matrix of a 3D vector.
+
+    Parameters:
+        v (array-like): A 3D vector.
+
+    Returns:
+        np.ndarray: The corresponding skew symmetric matrix.
     """
     return np.array([[0, -v[2], v[1]], [v[2], 0, -v[0]], [-v[1], v[0], 0]])
 
 def transform_from_twist(S, theta):
     """
     Computes the transformation matrix from a twist and a joint angle.
+
+    Parameters:
+        S (array-like): A 6D twist vector.
+        theta (float): The joint angle.
+
+    Returns:
+        np.ndarray: The corresponding transformation matrix.
     """
     omega = S[:3]
     v = S[3:]
     if np.linalg.norm(omega) == 0:  # Prismatic joint
         return np.vstack((np.eye(3), v * theta)).T
     else:  # Revolute joint
         skew_omega = skew_symmetric(omega)
         R = np.eye(3) + np.sin(theta) * skew_omega + (1 - np.cos(theta)) * np.dot(skew_omega, skew_omega)
         p = np.dot(np.eye(3) * theta + (1 - np.cos(theta)) * skew_omega + (theta - np.sin(theta)) * np.dot(skew_omega, skew_omega), v)
         return np.vstack((np.hstack((R, p.reshape(-1, 1))), [0, 0, 0, 1]))
 
 def adjoint_transform(T):
     """
     Computes the adjoint transformation matrix for a given transformation matrix.
+
+    Parameters:
+        T (np.ndarray): A 4x4 transformation matrix.
+
+    Returns:
+        np.ndarray: The corresponding adjoint transformation matrix.
     """
     R = T[0:3, 0:3]
     p = T[0:3, 3]
     skew_p = skew_symmetric(p)
     return np.vstack((np.hstack((R, np.zeros((3, 3)))), np.hstack((skew_p @ R, R))))
 
 def logm(T):
     """
     Computes the logarithm of a transformation matrix.
+
+    Parameters:
+        T (np.ndarray): A 4x4 transformation matrix.
+
+    Returns:
+        np.ndarray: The logarithm of the transformation matrix.
     """
     R = T[0:3, 0:3]
     p = T[0:3, 3]
     omega, theta = rotation_logm(R)
     if np.linalg.norm(omega) < 1e-6:
         v = p / theta
     else:
         G_inv = 1 / theta * np.eye(3) - 0.5 * skew_symmetric(omega) + (1 / theta - 0.5 / np.tan(theta / 2)) * np.dot(skew_symmetric(omega), skew_symmetric(omega))
         v = np.dot(G_inv, p)
     return np.hstack((omega * theta, v))
 
 def rotation_logm(R):
     """
     Computes the logarithm of a rotation matrix.
+
+    Parameters:
+        R (np.ndarray): A 3x3 rotation matrix.
+
+    Returns:
+        tuple: A tuple containing the rotation vector and the angle.
     """
     theta = np.arccos((np.trace(R) - 1) / 2)
     if theta < 1e-6:
         return np.zeros(3), theta
     else:
         omega = 1 / (2 * np.sin(theta)) * np.array([R[2, 1] - R[1, 2], R[0, 2] - R[2, 0], R[1, 0] - R[0, 1]])
         return omega, theta
+
 def logm_to_twist(logm):
     """
     Convert the logarithm of a transformation matrix to a twist vector.
 
     Parameters:
-        logm (numpy.darray): The logarithm of a transformation matrix.
+        logm (np.ndarray): The logarithm of a transformation matrix.
 
     Returns:
-        numpy.array: The corresponding twist vector.
+        np.ndarray: The corresponding twist vector.
     """
     if logm.shape != (4, 4):
         raise ValueError("logm must be a 4x4 matrix.")
-
-    # Extract the skew-symmetric part for angular velocity
+    
     omega_matrix = logm[0:3, 0:3]
     omega = skew_symmetric_to_vector(omega_matrix)
-
-    # Extract the linear velocity part
     v = logm[0:3, 3]
-
     return np.hstack((omega, v))
 
 def skew_symmetric_to_vector(skew_symmetric):
     """
     Convert a skew-symmetric matrix to a vector.
+
+    Parameters:
+        skew_symmetric (np.ndarray): A 3x3 skew-symmetric matrix.
+
+    Returns:
+        np.ndarray: The corresponding vector.
     """
     return np.array([skew_symmetric[2, 1], skew_symmetric[0, 2], skew_symmetric[1, 0]])
+
 def se3ToVec(se3_matrix):
     """
     Convert an se(3) matrix to a twist vector.
 
     Parameters:
-        se3_matrix (numpy.ndarray): A 4x4 matrix from the se(3) Lie algebra.
+        se3_matrix (np.ndarray): A 4x4 matrix from the se(3) Lie algebra.
 
     Returns:
-        numpy.ndarray: A 6-dimensional twist vector.
+        np.ndarray: A 6-dimensional twist vector.
     """
     if se3_matrix.shape != (4, 4):
         raise ValueError("Input matrix must be a 4x4 matrix.")
-
-    # Extract the angular velocity vector from the skew-symmetric part
+    
     omega = np.array([se3_matrix[2, 1], se3_matrix[0, 2], se3_matrix[1, 0]])
-
-    # Extract the linear velocity vector
     v = se3_matrix[0:3, 3]
+    return np.hstack((omega, v))
 
-    # Combine into a twist vector
-    twist = np.hstack((omega, v))
+def TransToRp(T):
+    """
+    Converts a homogeneous transformation matrix into a rotation matrix and position vector.
 
-    return twist
+    Parameters:
+        T (np.ndarray): A 4x4 transformation matrix.
 
-def TransToRp(T):
-    """Converts a homogeneous transformation matrix into a rotation matrix and position vector."""
+    Returns:
+        tuple: A tuple containing the rotation matrix and position vector.
+    """
     R = T[0:3, 0:3]
     p = T[0:3, 3]
     return R, p
 
 def TransInv(T):
-    """Inverts a homogeneous transformation matrix."""
+    """
+    Inverts a homogeneous transformation matrix.
+
+    Parameters:
+        T (np.ndarray): A 4x4 transformation matrix.
+
+    Returns:
+        np.ndarray: The inverse of the transformation matrix.
+    """
     R, p = TransToRp(T)
     Rt = R.T
     return np.vstack((np.hstack((Rt, -Rt @ p.reshape(-1, 1))), [0, 0, 0, 1]))
 
 def MatrixLog6(T):
-    """Computes the matrix logarithm of a homogeneous transformation matrix."""
+    """
+    Compute the matrix logarithm of a given transformation matrix T.
+
+    Parameters:
+        T (np.ndarray): The transformation matrix of shape (4, 4).
+        
+    Returns:
+        np.ndarray: The matrix logarithm of T, with shape (4, 4).
+    """
     R, p = TransToRp(T)
     omega, theta = rotation_logm(R)
     if np.linalg.norm(omega) < 1e-6:
         return np.vstack((np.hstack((np.zeros((3, 3)), p.reshape(-1, 1))), [0, 0, 0, 0]))
     else:
         omega_mat = skew_symmetric(omega)
         G_inv = 1 / theta * np.eye(3) - 0.5 * omega_mat + (1 / theta - 0.5 / np.tan(theta / 2)) * omega_mat @ omega_mat
         v = G_inv @ p
         return np.vstack((np.hstack((omega_mat, v.reshape(-1, 1))), [0, 0, 0, 0]))
 
-def rotation_logm(R):
-    """Computes the logarithm of a rotation matrix."""
-    theta = np.arccos((np.trace(R) - 1) / 2)
-    if theta < 1e-6:
-        return np.zeros(3), 0
-    else:
-        omega = (1 / (2 * np.sin(theta))) * np.array([R[2, 1] - R[1, 2], R[0, 2] - R[2, 0], R[1, 0] - R[0, 1]])
-        return omega, theta
-def MatrixLog6(T):
+def MatrixExp6(se3mat):
     """
-    Compute the matrix logarithm of a given transformation matrix T.
-    
+    Computes the matrix exponential of a matrix in se(3).
+
     Parameters:
-        T (ndarray): The transformation matrix of shape (4, 4).
-        
+        se3mat (np.ndarray): A 4x4 matrix representing a twist in se(3).
+
     Returns:
-        ndarray: The matrix logarithm of T, with shape (4, 4).
+        np.ndarray: The corresponding 4x4 transformation matrix in SE(3).
     """
-    R, p = TransToRp(T)
-    omgmat = MatrixLog3(R)
-    if np.array_equal(omgmat, np.zeros((3, 3))):
-        return np.r_[np.c_[np.zeros((3, 3)),
-                           [T[0][3], T[1][3], T[2][3]]],
-                     [[0, 0, 0, 0]]]
-    else:
-        theta = np.arccos((np.trace(R) - 1) / 2.0)
-        return np.r_[np.c_[omgmat,
-                           np.dot(np.eye(3) - omgmat / 2.0 \
-                           + (1.0 / theta - 1.0 / np.tan(theta / 2.0) / 2) \
-                              * np.dot(omgmat,omgmat) / theta,[T[0][3],
-                                                               T[1][3],
-                                                               T[2][3]])],
-                                                            [[0, 0, 0, 0]]]
+    if se3mat.shape != (4, 4):
+        raise ValueError("Input matrix must be of shape (4, 4)")
     
+    omega = np.array([se3mat[2, 1], se3mat[0, 2], se3mat[1, 0]])
+    v = np.array([se3mat[0, 3], se3mat[1, 3], se3mat[2, 3]])
+    omega_magnitude = np.linalg.norm(omega)
+
+    if omega_magnitude < 1e-6:
+        return np.eye(4) + se3mat
+
+    omega_skew = skew_symmetric(omega)
+    omega_exp = expm(omega_skew * omega_magnitude)
+    omega_skew_squared = np.dot(omega_skew, omega_skew)
+    v_term = (np.eye(3) * omega_magnitude + (1 - np.cos(omega_magnitude)) * omega_skew + (omega_magnitude - np.sin(omega_magnitude)) * omega_skew_squared) / omega_magnitude**2
+    v_term = np.dot(v_term, v)
+
+    T = np.eye(4)
+    T[:3, :3] = omega_exp
+    T[:3, 3] = v_term
+
+    return T
+
 def MatrixLog3(R):
-    
+    """
+    Computes the matrix logarithm of a rotation matrix.
+
+    Parameters:
+        R (np.ndarray): A 3x3 rotation matrix.
+
+    Returns:
+        np.ndarray: The matrix logarithm of the rotation matrix.
+    """
     acosinput = (np.trace(R) - 1) / 2.0
     if acosinput >= 1:
         return np.zeros((3, 3))
     elif acosinput <= -1:
         if not NearZero(1 + R[2][2]):
-            omg = (1.0 / np.sqrt(2 * (1 + R[2][2]))) \
-                  * np.array([R[0][2], R[1][2], 1 + R[2][2]])
+            omega = (1.0 / np.sqrt(2 * (1 + R[2][2]))) * np.array([R[0][2], R[1][2], 1 + R[2][2]])
         elif not NearZero(1 + R[1][1]):
-            omg = (1.0 / np.sqrt(2 * (1 + R[1][1]))) \
-                  * np.array([R[0][1], 1 + R[1][1], R[2][1]])
+            omega = (1.0 / np.sqrt(2 * (1 + R[1][1]))) * np.array([R[0][1], 1 + R[1][1], R[2][1]])
         else:
-            omg = (1.0 / np.sqrt(2 * (1 + R[0][0]))) \
-                  * np.array([1 + R[0][0], R[1][0], R[2][0]])
-        return VecToso3(np.pi * omg)
+            omega = (1.0 / np.sqrt(2 * (1 + R[0][0]))) * np.array([1 + R[0][0], R[1][0], R[2][0]])
+        return VecToso3(np.pi * omega)
     else:
         theta = np.arccos(acosinput)
         return theta / 2.0 / np.sin(theta) * (R - np.array(R).T)
-    
 
-def VecToso3(omg):
-   
-    return np.array([[0,      -omg[2],  omg[1]],
-                     [omg[2],       0, -omg[0]],
-                     [-omg[1], omg[0],       0]])
-def VecTose3(V):
-    
-    return np.r_[np.c_[VecToso3([V[0], V[1], V[2]]), [V[3], V[4], V[5]]],
-                 np.zeros((1, 4))]
+def VecToso3(omega):
+    """
+    Converts a 3D angular velocity vector to a skew-symmetric matrix.
 
-def MatrixExp6(se3mat):
+    Parameters:
+        omega (array-like): A 3D angular velocity vector.
+
+    Returns:
+        np.ndarray: The corresponding skew-symmetric matrix.
     """
-    Computes the matrix exponential of a matrix in se(3).
+    return np.array([[0, -omega[2], omega[1]], [omega[2], 0, -omega[0]], [-omega[1], omega[0], 0]])
+
+def VecTose3(V):
+    """
+    Converts a spatial velocity vector to an se(3) matrix.
 
     Parameters:
-    se3mat (np.ndarray): A 4x4 matrix representing a twist in se(3).
+        V (array-like): A 6D spatial velocity vector.
 
     Returns:
-    np.ndarray: The corresponding 4x4 transformation matrix in SE(3).
+        np.ndarray: The corresponding 4x4 matrix in se(3).
     """
-    if se3mat.shape != (4, 4):
-        raise ValueError("Input matrix must be of shape (4, 4)")
+    return np.r_[np.c_[VecToso3(V[:3]), V[3:].reshape(3, 1)], np.zeros((1, 4))]
+def MatrixExp3(so3mat):
+    """
+    Computes the matrix exponential of a matrix in so(3).
 
-    # Extract the angular velocity vector (omega) and linear velocity vector (v) from the se3 matrix
-    omega = np.array([se3mat[2, 1], se3mat[0, 2], se3mat[1, 0]])
-    v = np.array([se3mat[0, 3], se3mat[1, 3], se3mat[2, 3]])
+    Parameters:
+        so3mat (np.ndarray): A 3x3 skew-symmetric matrix.
 
-    # Compute the magnitude of omega
-    omega_magnitude = np.linalg.norm(omega)
+    Returns:
+        np.ndarray: The corresponding 3x3 rotation matrix in SO(3).
+    """
+    return expm(so3mat)
 
-    if omega_magnitude < 1e-6:
-        # If omega is very small, use the first-order Taylor expansion of matrix exponential
-        return np.eye(4) + se3mat
+def CubicTimeScaling(Tf, t):
+    """
+    Compute the cubic time scaling factor.
 
-    # Compute the skew-symmetric matrix of omega
-    omega_skew = skew_symmetric(omega)
+    Parameters:
+        Tf (float): The total time of the motion.
+        t (float): The current time.
 
-    # Compute the matrix exponential of the skew-symmetric matrix of omega
-    omega_exp = expm(omega_skew * omega_magnitude)
+    Returns:
+        float: The cubic time scaling factor.
+    """
+    return 3 * (t / Tf) ** 2 - 2 * (t / Tf) ** 3
 
-    # Compute the additional term for the linear velocity part
-    omega_skew_squared = np.dot(omega_skew, omega_skew)
-    v_term = (np.eye(3) * omega_magnitude + (1 - np.cos(omega_magnitude)) * omega_skew + (omega_magnitude - np.sin(omega_magnitude)) * omega_skew_squared) / omega_magnitude**2
-    v_term = np.dot(v_term, v)
+def QuinticTimeScaling(Tf, t):
+    """
+    Compute the quintic time scaling factor.
 
-    # Construct the final transformation matrix
-    T = np.eye(4)
-    T[:3, :3] = omega_exp
-    T[:3, 3] = v_term
+    Parameters:
+        Tf (float): The total time of the motion.
+        t (float): The current time.
 
-    return T
+    Returns:
+        float: The quintic time scaling factor.
+    """
+    return 10 * (t / Tf) ** 3 - 15 * (t / Tf) ** 4 + 6 * (t / Tf) ** 5
```

### Comparing `ManipulaPy-1.0.0.2/setup.py` & `ManipulaPy-1.0.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #!/usr/bin/env python3
 
 
 from setuptools import setup, find_packages
 
 setup(
     name='ManipulaPy',
-    version='1.0.0.2',
+    version='1.0.1',
     author='Mohamed Aboelnar',
     author_email='aboelnasr1997@gmail.com',  # Optional
     description='A package for robotic serial manipulator operations',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',  # if your README is in markdown
     url='https://github.com/boelnasr/ManipulaPy',  # Optional
     packages=find_packages(),
     install_requires=[
-        # Add your package dependencies here
-        'numpy',
-        'scipy',
-        'urchin',
-        'pybullet'
-        # 'pybullet', # If this is a dependency, it should be listed here
-    ],
+    'numpy>=1.19.2',
+    'scipy>=1.5.2',
+    'urchin>=0.9.0',
+    'pybullet>=3.0.6',
+    'pycuda>=2021.1'
+        ],
+
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
 )
```

