# Comparing `tmp/sapiopycommons-31.3.0.23.12.3.tar.gz` & `tmp/sapiopycommons-32.0.0.24.5.tar.gz`

## Comparing `sapiopycommons-31.3.0.23.12.3.tar` & `sapiopycommons-32.0.0.24.5.tar`

### file list

```diff
@@ -1,33 +1,48 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/__init__.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/chem/IndigoMolecules.py
--rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/chem/Molecules.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/chem/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/datatype/__init__.py
--rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/datatype/attachment_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/eln/__init__.py
--rw-r--r--   0        0        0    57231 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/eln/experiment_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/files/__init__.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/files/complex_data_loader.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/files/file_bridge.py
--rw-r--r--   0        0        0    23383 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/files/file_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/__init__.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/aliases.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/custom_report_util.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/exceptions.py
--rw-r--r--   0        0        0    29112 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/popup_util.py
--rw-r--r--   0        0        0     8892 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/storage_util.py
--rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/time_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/processtracking/__init__.py
--rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/processtracking/endpoints.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/recordmodel/__init__.py
--rw-r--r--   0        0        0    35178 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/recordmodel/record_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/rules/__init__.py
--rw-r--r--   0        0        0     9997 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/rules/eln_rule_handler.py
--rw-r--r--   0        0        0    10126 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/rules/on_save_rule_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/webhook/__init__.py
--rw-r--r--   0        0        0    11794 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/webhook/webhook_handlers.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/LICENSE
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/README.md
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/pyproject.toml
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/callbacks/__init__.py
+-rw-r--r--   0        0        0    43256 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/callbacks/callback_util.py
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/chem/IndigoMolecules.py
+-rw-r--r--   0        0        0     8639 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/chem/Molecules.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/chem/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/datatype/__init__.py
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/datatype/attachment_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/eln/__init__.py
+-rw-r--r--   0        0        0    57198 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/eln/experiment_handler.py
+-rw-r--r--   0        0        0     7184 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/eln/plate_designer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/__init__.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/complex_data_loader.py
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/file_bridge.py
+-rw-r--r--   0        0        0    36746 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/file_data_handler.py
+-rw-r--r--   0        0        0    25556 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/file_util.py
+-rw-r--r--   0        0        0    24499 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/file_validator.py
+-rw-r--r--   0        0        0    16027 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/file_writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/__init__.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/aliases.py
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/custom_report_util.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/exceptions.py
+-rw-r--r--   0        0        0    30126 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/popup_util.py
+-rw-r--r--   0        0        0     8892 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/storage_util.py
+-rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/time_util.py
+-rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/multimodal/multimodal.py
+-rw-r--r--   0        0        0    14787 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/multimodal/multimodal_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/processtracking/__init__.py
+-rw-r--r--   0        0        0    10926 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/processtracking/endpoints.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/recordmodel/__init__.py
+-rw-r--r--   0        0        0    39348 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/recordmodel/record_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/rules/__init__.py
+-rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/rules/eln_rule_handler.py
+-rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/rules/on_save_rule_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/webhook/__init__.py
+-rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/webhook/webhook_handlers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/tests/_do_not_add_init_py_here
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/tests/bio_reg_test.py
+-rw-r--r--   0        0        0    12222 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/tests/chem_test.py
+-rw-r--r--   0        0        0  1669824 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/tests/data_type_models.py
+-rw-r--r--   0        0        0    10718 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/tests/kappa.chains.fasta
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/tests/mafft_test.py
+-rw-r--r--   0        0        0     6063 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/tests/test.gb
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/LICENSE
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/README.md
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/pyproject.toml
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/PKG-INFO
```

### Comparing `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/chem/IndigoMolecules.py` & `sapiopycommons-32.0.0.24.5/src/sapiopycommons/chem/IndigoMolecules.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from indigo.inchi import IndigoInchi
 from indigo.renderer import IndigoRenderer
 
 indigo = Indigo()
 renderer = IndigoRenderer(indigo)
 indigo.setOption("render-output-format", "svg")
 indigo.setOption("ignore-stereochemistry-errors", True)
+indigo.setOption("render-stereo-style", "ext")
 indigo.setOption("aromaticity-model", "generic")
 indigo.setOption("render-coloring", True)
 indigo_inchi = IndigoInchi(indigo);
 
 
 def highlight_mol_substructure(query: IndigoObject, sub_match: IndigoObject):
     """
```

### Comparing `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/chem/Molecules.py` & `sapiopycommons-32.0.0.24.5/src/sapiopycommons/chem/Molecules.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,14 +177,15 @@
         img = mol_to_img(smiles)
         molecule["image"] = img
     else:
         molecule["image"] = None
     # We need to test the INCHI can be loaded back to indigo.
     indigo_mol = indigo.loadMolecule(molBlock)
     indigo_mol.aromatize()
+    indigo_inchi.resetOptions()
     indigo_inchi_str = indigo_inchi.getInchi(indigo_mol)
     molecule["inchi"] = indigo_inchi_str
     indigo_inchi_key_str = indigo_inchi.getInchiKey(indigo_inchi_str)
     molecule["inchiKey"] = indigo_inchi_key_str
     molecule["smiles"] = indigo_mol.smiles()
 
     if include_stereoisomers and has_chiral_centers(mol):
```

### Comparing `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/datatype/attachment_util.py` & `sapiopycommons-32.0.0.24.5/src/sapiopycommons/datatype/attachment_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import io
 
-from sapiopylib.rest.pojo.DataRecord import DataRecord
+from sapiopylib.rest.User import SapioUser
 from sapiopylib.rest.pojo.webhook.WebhookContext import SapioWebhookContext
-from sapiopylib.rest.utils.recordmodel.RecordModelManager import RecordModelManager
 from sapiopylib.rest.utils.recordmodel.RecordModelWrapper import WrappedType
 
 from sapiopycommons.general.aliases import AliasUtil, SapioRecord
 from sapiopycommons.general.exceptions import SapioException
+from sapiopycommons.recordmodel.record_handler import RecordHandler
 
 
 # FR-46064 - Initial port of PyWebhookUtils to sapiopycommons.
 class AttachmentUtil:
     @staticmethod
     def get_attachment_bytes(context: SapioWebhookContext, attachment: SapioRecord) -> bytes:
         """
@@ -45,24 +45,22 @@
             raise SapioException("Provided record cannot have its attachment data set, as it does not exist in the "
                                  "system yet.")
         attachment = AliasUtil.to_data_record(attachment)
         with io.BytesIO(file_bytes) as stream:
             context.data_record_manager.set_attachment_data(attachment, file_name, stream)
 
     @staticmethod
-    def create_attachment(context: SapioWebhookContext, file_name: str, file_bytes: bytes,
+    def create_attachment(context: SapioWebhookContext | SapioUser, file_name: str, file_bytes: bytes,
                           wrapper_type: type[WrappedType]) -> WrappedType:
         """
         Create an attachment data type and initialize its attachment bytes at the same time.
         Makes a webservice call to create the attachment record and a second to set its bytes.
 
-        :param context: The current webhook context.
+        :param context: The current webhook context or a user object to send requests from.
         :param file_name: The name of the attachment.
         :param file_bytes: THe bytes of the attachment data.
         :param wrapper_type: The attachment type to create.
         :return: A record model for the newly created attachment.
         """
-        inst_man = RecordModelManager(context.user).instance_manager
-        attachment: DataRecord = context.data_record_manager.add_data_record(wrapper_type.DATA_TYPE_NAME)
-        attachment: WrappedType = inst_man.add_existing_record_of_type(attachment, wrapper_type)
+        attachment: WrappedType = RecordHandler(context).create_models(wrapper_type, 1)[0]
         AttachmentUtil.set_attachment_bytes(context, attachment, file_name, file_bytes)
         return attachment
```

### Comparing `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/eln/experiment_handler.py` & `sapiopycommons-32.0.0.24.5/src/sapiopycommons/eln/experiment_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 Step = str | ElnEntryStep
 """An object representing an identifier to an ElnEntryStep. May be either the name of the step or the ElnEntryStep
 itself."""
 
 
 # FR-46064 - Initial port of PyWebhookUtils to sapiopycommons.
 class ExperimentHandler:
-    __context: SapioWebhookContext
+    context: SapioWebhookContext
     """The context that this handler is working from."""
 
     # Basic experiment info from the context.
     __eln_exp: ElnExperiment
     """The ELN experiment from the context."""
     __protocol: ElnExperimentProtocol
     """The ELN experiment as a protocol."""
@@ -60,22 +60,19 @@
     __steps: dict[str, ElnEntryStep]
     """Steps from this experiment. All steps are cached the first time any individual step is accessed."""
     __step_options: dict[ElnEntryStep, dict[str, str]]
     """Entry options for each step in this experiment. Only cached for each individual step when they are first accessed.
     The cache is updated whenever the entry options for a step are changed by this handler."""
 
     # Constants
-    # TODO: sapiopylib is currently storing the status of entries as strings when first queried, requiring us to compare
-    #  against the value of the enums instead of the enums themselves. The ".value"s can be removed once sapiopylib is
-    #  fixed.
-    __ENTRY_COMPLETE_STATUSES = [ExperimentEntryStatus.Completed.value, ExperimentEntryStatus.CompletedApproved.value]
+    __ENTRY_COMPLETE_STATUSES = [ExperimentEntryStatus.Completed, ExperimentEntryStatus.CompletedApproved]
     """The set of statuses that an ELN entry could have and be considered completed/submitted."""
-    __ENTRY_LOCKED_STATUSES = [ExperimentEntryStatus.Completed.value, ExperimentEntryStatus.CompletedApproved.value,
-                               ExperimentEntryStatus.Disabled.value, ExperimentEntryStatus.LockedAwaitingApproval.value,
-                               ExperimentEntryStatus.LockedRejected.value]
+    __ENTRY_LOCKED_STATUSES = [ExperimentEntryStatus.Completed, ExperimentEntryStatus.CompletedApproved,
+                               ExperimentEntryStatus.Disabled, ExperimentEntryStatus.LockedAwaitingApproval,
+                               ExperimentEntryStatus.LockedRejected]
     """The set of statuses that an ELN entry could have and be considered locked."""
     __EXPERIMENT_COMPLETE_STATUSES = [ElnExperimentStatus.Completed, ElnExperimentStatus.CompletedApproved]
     """The set of statuses that an ELN experiment could have and be considered completed."""
     __EXPERIMENT_LOCKED_STATUSES = [ElnExperimentStatus.Completed, ElnExperimentStatus.CompletedApproved,
                                     ElnExperimentStatus.LockedRejected, ElnExperimentStatus.LockedAwaitingApproval,
                                     ElnExperimentStatus.Canceled]
     """The set of statuses that an ELN experiment could have and be considered locked."""
@@ -91,15 +88,15 @@
         """
         # FR-46495 - Allow the init function of ExperimentHandler to take in an ElnExperiment that is separate from the
         # context.
         if context.eln_experiment is None and experiment is None:
             raise SapioException("Cannot initialize ExperimentHandler. No ELN Experiment in the context.")
         if context.eln_experiment == experiment:
             experiment = None
-        self.__context = context
+        self.context = context
 
         # Get the basic information about this experiment that already exists in the context and is often used.
         self.__eln_exp = experiment if experiment else context.eln_experiment
         self.__protocol = ElnExperimentProtocol(experiment, context.user) if experiment else context.active_protocol
         self.__exp_id = self.__protocol.get_id()
 
         # Grab various managers that may be used.
@@ -262,15 +259,15 @@
         Query for the data record of this experiment. The returned record is cached by the ExperimentHandler.
 
         :param exception_on_none: If false, returns None if there is no experiment record. If true, raises an exception
             when the experiment record doesn't exist.
         :return: The data record for this experiment. None if it has no record.
         """
         if not hasattr(self, "_ExperimentHandler__exp_record"):
-            drm = self.__context.data_record_manager
+            drm = self.context.data_record_manager
             dt = self.__eln_exp.experiment_data_type_name
             results = drm.query_data_records_by_id(dt, [self.__eln_exp.experiment_record_id]).result_list
             # PR-46504: Set the exp_record to None if there are no results.
             self.__exp_record = results[0] if results else None
         if self.__exp_record is None and exception_on_none:
             raise SapioException(f"Experiment record not found for experiment with ID {self.__exp_id}.")
         return self.__exp_record
@@ -466,14 +463,34 @@
 
             step: ElnEntryStep = self.__steps.get(name)
             if step is None and exception_on_none is True:
                 raise SapioException(f"ElnEntryStep of name \"{name}\" not found in experiment with ID {self.__exp_id}.")
             ret_list.append(step)
         return ret_list
 
+    def get_all_steps(self, data_type: str | type[WrappedType] | None = None) -> list[ElnEntryStep]:
+        """
+        Get a list of every entry in the experiment. Optionally filter the returned entries by a data type.
+
+        Makes a webservice call to retrieve every entry in the experiment if they were not already previously cached.
+
+        :param data_type: A data type used to filter the returned entries. If None is given, returns all entries. If
+            a data type name or wrapper is given, only returns entries that match that data type name or wrapper.
+        :return: Every entry in the experiment in order of appearance that match the provided data type, if any.
+        """
+        if self.__queried_all_steps is False:
+            self.__queried_all_steps = True
+            self.__steps.update({step.get_name(): step for step in self.__protocol.get_sorted_step_list()})
+        all_steps: list[ElnEntryStep] = self.__protocol.get_sorted_step_list()
+        if data_type is None:
+            return all_steps
+        if not isinstance(data_type, str):
+            data_type: str = data_type.get_wrapper_data_type_name()
+        return [x for x in all_steps if data_type in x.get_data_type_names()]
+
     def get_step_records(self, step: Step) -> list[DataRecord]:
         """
         Query for the data records for the given step. The returned records are not cached by the ExperimentHandler.
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
 
@@ -762,18 +779,15 @@
             entry.entry_name = entry_name
             self.__steps.update({entry_name: step})
         if related_entry_set is not None:
             entry.related_entry_id_set = related_entry_set
         if dependency_set is not None:
             entry.dependency_set = dependency_set
         if entry_status is not None:
-            # TODO: sapiopylib is currently storing the status of entries as strings when first queried. For the sake of not
-            #  breaking comparisons to enums that expect this behavior, also setting the status to the enum's string.
-            #  The ".value" can be removed once sapiopylib is fixed.
-            entry.entry_status = entry_status.value
+            entry.entry_status = entry_status
         if order is not None:
             entry.order = order
         if description is not None:
             entry.description = description
         if requires_grabber_plugin is not None:
             entry.requires_grabber_plugin = requires_grabber_plugin
         if is_initialization_required is not None:
@@ -918,18 +932,15 @@
             The step to complete.
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         """
         step = self.__to_eln_step(step)
         if step.eln_entry.entry_status not in self.__ENTRY_COMPLETE_STATUSES:
             step.complete_step()
-            # TODO: sapiopylib is currently storing the status of entries as strings when first queried. For the sake of not
-            #  breaking comparisons to enums that expect this behavior, also setting the status to the enum's string.
-            #  The ".value" can be removed once sapiopylib is fixed.
-            step.eln_entry.entry_status = ExperimentEntryStatus.Completed.value
+            step.eln_entry.entry_status = ExperimentEntryStatus.Completed
 
     def unlock_step(self, step: Step) -> None:
         """
         Set the status of the input step to UnlockedChangesRequired. Makes a webservice call to update the step. Checks
         if the step is already unlocked, and does nothing if so.
 
         If no step functions have been called before and a step is being searched for by name, queries for the
@@ -939,18 +950,15 @@
             The step to unlock.
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         """
         step = self.__to_eln_step(step)
         if step.eln_entry.entry_status in self.__ENTRY_LOCKED_STATUSES:
             step.unlock_step()
-            # TODO: sapiopylib is currently storing the status of entries as strings when first queried. For the sake of not
-            #  breaking comparisons to enums that expect this behavior, also setting the status to the enum's string.
-            #  The ".value" can be removed once sapiopylib is fixed.
-            step.eln_entry.entry_status = ExperimentEntryStatus.UnlockedChangesRequired.value
+            step.eln_entry.entry_status = ExperimentEntryStatus.UnlockedChangesRequired
 
     def step_is_submitted(self, step: Step) -> bool:
         """
         Determine if the input step has already been submitted.
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
```

### Comparing `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/files/complex_data_loader.py` & `sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/complex_data_loader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import io
 
+from sapiopylib.rest.User import SapioUser
 from sapiopylib.rest.pojo.webhook.WebhookContext import SapioWebhookContext
 
 
 class CDL:
     @staticmethod
-    def load_cdl(context: SapioWebhookContext, config_name: str, file_name: str, file_data: bytes | str) \
+    def load_cdl(context: SapioWebhookContext | SapioUser, config_name: str, file_name: str, file_data: bytes | str) \
             -> list[int]:
         """
         Create data records from a file using one of the complex data loader (CDL) configurations in the system.
 
-        :param context: The current webhook context.
+        :param context: The current webhook context or a user object to send requests from.
         :param config_name: The name of the CDL configuration to run.
         :param file_name: The name of the file being read by the CDL.
         :param file_data: A string or bytes of the file to be read by the CDL.
         :return: A list of the record IDs of the data records created by the CDL.
         """
         sub_path = "/ext/cdl/load"
         params = {
             "configName": config_name,
             "fileName": file_name
         }
+        user: SapioUser = context if isinstance(context, SapioUser) else context.user
         with io.StringIO(file_data) if isinstance(file_data, str) else io.BytesIO(file_data) as data_stream:
-            response = context.user.post_data_stream(sub_path, params=params, data_stream=data_stream)
-        context.user.raise_for_status(response)
+            response = user.post_data_stream(sub_path, params=params, data_stream=data_stream)
+        user.raise_for_status(response)
         # The response content is returned as bytes for a comma separated string of record IDs.
         return [int(x) for x in bytes.decode(response.content).split(",")]
```

### Comparing `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/files/file_util.py` & `sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/file_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,191 +9,42 @@
 from sapiopylib.rest.pojo.webhook.WebhookContext import SapioWebhookContext
 from sapiopylib.rest.pojo.webhook.WebhookResult import SapioWebhookResult
 
 from sapiopycommons.general.exceptions import SapioUserErrorException
 
 
 # FR-46064 - Initial port of PyWebhookUtils to sapiopycommons.
+# FR-46716 - Add comments noting that some functions are deprecated in favor of CallbackUtil.
 class FileUtil:
     """
     Utilities for the handling of files, including the requesting of files from the user and the parsing of files into
     tokenized lists. Makes use of Pandas DataFrames for any file parsing purposes.
     """
-    # FR-46097 - Add write file request shorthand functions to FileUtil.
-    @staticmethod
-    def write_file(file_name: str, file_bytes: bytes, *, request_context: str | None = None) -> SapioWebhookResult:
-        """
-        Send a file to the client.
-
-        The calling webhook must catch the WriteFileResult that the client will send back.
-
-        :param file_name: The name of the file.
-        :param file_bytes: The bytes of the file.
-        :param request_context: Context that will be returned to the webhook server in the client callback result.
-        :return: A SapioWebhookResult with the write request as its client callback request.
-        """
-        return SapioWebhookResult(True, client_callback_request=WriteFileRequest(file_bytes, file_name,
-                                                                                 request_context))
-
-    @staticmethod
-    def write_files(files: dict[str, bytes], *, request_context: str | None = None) -> SapioWebhookResult:
-        """
-        Send a collection of files to the client.
-
-        The calling webhook must catch the MultiFileResult that the client will send back.
-
-        :param files: A dictionary of files names to file bytes.
-        :param request_context: Context that will be returned to the webhook server in the client callback result.
-        :return: A SapioWebhookResult with the write request as its client callback request.
-        """
-        return SapioWebhookResult(True, client_callback_request=MultiFileRequest(files, request_context))
-
-    @staticmethod
-    def request_file(context: SapioWebhookContext, title: str, exts: list[str] = None,
-                     *, request_context: str | None = None) \
-            -> tuple[SapioWebhookResult | None, str | None, bytes | None]:
-        """
-        Request a single file from the user. This function handles the entire client callback interaction for the
-        requesting of the file, including if the user cancels the file upload prompt.
-
-        The first time this method is called in the course of an interaction with the client, it will return a webhook
-        result containing the client callback to request the file. The second time it is called, it will return the
-        file name and bytes from the callback result.
-
-        :param context: The current webhook context.
-        :param title: The title of the file prompt dialog.
-        :param exts: The allowable file extensions of the uploaded file. If blank, any file can be uploaded. Throws an
-            exception if an incorrect file extension is provided.
-        :param request_context: Context that will be returned to the webhook server in the client callback result.
-        :return: A tuple with the following elements.
-            0 - A webhook result that contains a file prompt if this is the first interaction with this request.
-            May also contain a result that will terminate the client interaction if the user canceled the prompt.
-            1 - The file name of the requested file if the user provided one.
-            2 - The file bytes of the requested file if the user provided one.
-        """
-        client_callback = context.client_callback_result
-        result_context: str | None = client_callback.callback_context_data if client_callback else None
-        # If the user cancels, terminate the interaction.
-        if client_callback is not None and client_callback.user_cancelled:
-            return SapioWebhookResult(True), None, None
-        # If no extensions were provided, use an empty list for the extensions instead.
-        if exts is None:
-            exts = []
-
-        # If the client callback isn't a FilePromptResult, then it's either None or some other callback result, meaning
-        # we need to send a new request. We may also send a new request if the client callback result is a
-        # FilePromptResult, but its callback context doesn't match the provided callback context, meaning it's a
-        # result from a different call to request_file.
-        is_file_result = isinstance(client_callback, FilePromptResult)
-        if not is_file_result or (is_file_result and result_context != request_context):
-            prompt = FilePromptRequest(dialog_title=title, file_extension=",".join(exts),
-                                       callback_context_data=request_context)
-            return SapioWebhookResult(True, client_callback_request=prompt), None, None
-
-        # Get the file from the result. Enforce that the provided data isn't empty, and that the file path ends in
-        # one of the allowed extensions.
-        # noinspection PyTypeChecker
-        result: FilePromptResult = client_callback
-        file_path: str | None = result.file_path
-        file_bytes: bytes | None = result.file_bytes
-        FileUtil.__verify_file(file_path, file_bytes, exts)
-        return None, file_path, file_bytes
-
-    @staticmethod
-    def request_files(context: SapioWebhookContext, title: str, exts: list[str] = None,
-                      *, request_context: str | None = None) \
-            -> tuple[SapioWebhookResult | None, dict[str, bytes] | None]:
-        """
-        Request multiple files from the user. This function handles the entire client callback interaction for the
-        requesting of the files, including if the user cancels the file upload prompt.
-
-        The first time this method is called in the course of an interaction with the client, it will return a webhook
-        result containing the client callback to request the files. The second time it is called, it will return each
-        file name and bytes from the callback result.
-
-        :param context: The current webhook context.
-        :param title: The title of the file prompt dialog.
-        :param exts: The allowable file extensions of the uploaded file. If blank, any file can be uploaded. Throws an
-            exception if an incorrect file extension is provided.
-        :param request_context: Context that will be returned to the webhook server in the client callback result.
-        :return: A tuple with the following elements.
-            0 - A webhook result that contains a file prompt if this is the first interaction with this request.
-            May also contain a result that will terminate the client interaction if the user canceled the prompt.
-            1 - A dictionary that maps the file names to the file bytes for each provided file.
-        """
-        client_callback = context.client_callback_result
-        result_context: str | None = client_callback.callback_context_data if client_callback else None
-        # If the user cancels, terminate the interaction.
-        if client_callback is not None and client_callback.user_cancelled:
-            return SapioWebhookResult(True), None
-        # If no extensions were provided, use an empty list for the extensions instead.
-        if exts is None:
-            exts = []
-
-        # If the client callback isn't a MultiFilePromptResult, then it's either None or some other callback result,
-        # meaning we need to send a new request. We may also send a new request if the client callback result is a
-        # MultiFilePromptResult, but its callback context doesn't match the provided callback context, meaning it's a
-        # result from a different call to request_file.
-        is_file_result = isinstance(client_callback, MultiFilePromptResult)
-        if not is_file_result or (is_file_result and result_context != request_context):
-            prompt = MultiFilePromptRequest(dialog_title=title, file_extension=",".join(exts),
-                                            callback_context_data=request_context)
-            return SapioWebhookResult(True, client_callback_request=prompt), None
-
-        # Get the files from the result. Enforce that the provided data isn't empty, and that the file paths end in
-        # one of the allowed extensions.
-        # noinspection PyTypeChecker
-        result: MultiFilePromptResult = client_callback
-        for file_path, file_bytes in result.files.items():
-            FileUtil.__verify_file(file_path, file_bytes, exts)
-        return None, result.files
-
     @staticmethod
-    def __verify_file(file_path: str, file_bytes: bytes, allowed_extensions: list[str]):
-        """
-        Verify that the provided file was read (i.e. the file path and file bytes aren't None or empty) and that it
-        has the correct file extension. Raises a user error exception if something about the file is incorrect.
-
-        :param file_path: The name of the file to verify.
-        :param file_bytes: The bytes of the file to verify.
-        :param allowed_extensions: The file extensions that the file path is allowed to have.
-        """
-        if file_path is None or len(file_path) == 0 or file_bytes is None or len(file_bytes) == 0:
-            raise SapioUserErrorException("Empty file provided or file unable to be read.")
-        if len(allowed_extensions) != 0:
-            matches: bool = False
-            for ext in allowed_extensions:
-                if file_path.endswith("." + ext):
-                    matches = True
-                    break
-            if matches is False:
-                raise SapioUserErrorException("Unsupported file type. Expecting the following extension(s): "
-                                              + (",".join(allowed_extensions)))
-
-    @staticmethod
-    def tokenize_csv(file_bytes: bytes, required_headers: list[str] | None = None, header_row_index: int | None = 0) \
-            -> tuple[list[dict[str, str]], list[list[str]]]:
+    def tokenize_csv(file_bytes: bytes, required_headers: list[str] | None = None, header_row_index: int | None = 0,
+                     seperator: str = ",") -> tuple[list[dict[str, str]], list[list[str]]]:
         """
         Tokenize a CSV file. The provided file must be uniform. That is, if row 1 has 10 cells, all the rows in the file
         must have 10 cells. Otherwise, the Pandas parser throws a tokenizer exception.
 
         :param file_bytes: The bytes of the CSV to be parsed.
         :param required_headers: The headers that must be present in the file. If a provided header is missing, raises
             a user error exception.
         :param header_row_index: The row index in the file that the headers are located at. Everything above the header
             row is returned in the metadata list. If input is None, then no row is considered to be the header row,
             meaning that required headers are also ignored if any are provided. By default, the first row (0th index)
             is assumed to be the header row.
+        :param seperator: The character that separates cells in the table.
         :return: The CSV parsed into a list of dicts where each dict is a row, mapping the headers to the cells for
             that row. Also returns a list of each row above the headers (the metadata), parsed into a list of each cell.
             If the header row index is 0 or None, this list will be empty.
         """
         # Parse the file bytes into two DataFrames. The first is metadata of the file located above the header row,
         # while the second is the body of the file below the header row.
-        file_body, file_metadata = FileUtil.csv_to_data_frames(file_bytes, header_row_index)
+        file_body, file_metadata = FileUtil.csv_to_data_frames(file_bytes, header_row_index, seperator)
         # Parse the metadata from above the header row index into a list of lists.
         metadata: list[list[str]] = FileUtil.data_frame_to_lists(file_metadata)
         # Parse the data from the file body into a list of dicts.
         rows: list[dict[str, str]] = FileUtil.data_frame_to_dicts(file_body, required_headers, header_row_index)
         return rows, metadata
 
     @staticmethod
@@ -219,43 +70,44 @@
         # Parse the metadata from above the header row index into a list of lists.
         metadata: list[list[str]] = FileUtil.data_frame_to_lists(file_metadata)
         # Parse the data from the file body into a list of dicts.
         rows: list[dict[str, str]] = FileUtil.data_frame_to_dicts(file_body, required_headers, header_row_index)
         return rows, metadata
 
     @staticmethod
-    def csv_to_data_frames(file_bytes: bytes, header_row_index: int | None = 0) \
+    def csv_to_data_frames(file_bytes: bytes, header_row_index: int | None = 0, seperator: str = ",") \
             -> tuple[DataFrame, DataFrame | None]:
         """
         Parse the file bytes for a CSV into DataFrames. The provided file must be uniform. That is, if row 1 has 10
         cells, all the rows in the file must have 10 cells. Otherwise, the Pandas parser throws a tokenizer exception.
 
         :param file_bytes: The bytes of the CSV to be parsed.
         :param header_row_index: The row index in the file that the headers are located at. Everything above the header
             row is returned in the metadata list. If input is None, then no row is considered to be the header row,
             meaning that required headers are also ignored if any are provided. By default, the first row (0th index)
             is assumed to be the header row.
+        :param seperator: The character that separates cells in the table.
         :return: A tuple of two DataFrames. The first is the frame for the CSV table body, while the second is for the
             metadata from above the header row, or None if there is no metadata.
         """
         file_metadata: DataFrame | None = None
         if header_row_index is not None and header_row_index > 0:
             with io.BytesIO(file_bytes) as file_io:
                 # The metadata DataFrame has no headers and only consists of the rows above the header row index.
                 # Therefore, we skip every row including and past the header. Don't skip blank rows, as skipping them
                 # can throw off the header row index.
                 file_metadata = pandas.read_csv(file_io, header=None, dtype=dtype(str),
                                                 skiprows=lambda x: x >= header_row_index,
-                                                skip_blank_lines=False)
+                                                skip_blank_lines=False, sep=seperator)
         with io.BytesIO(file_bytes) as file_io:
             # The use of the dtype argument is to ensure that everything from the file gets read as a string. Added
             # because some numerical values would get ".0" appended to them, even when casting the DataFrame cell to a
             # string.
             file_body: DataFrame = pandas.read_csv(file_io, header=header_row_index, dtype=dtype(str),
-                                                   skip_blank_lines=False)
+                                                   skip_blank_lines=False, sep=seperator)
 
         return file_body, file_metadata
 
     @staticmethod
     def xlsx_to_data_frames(file_bytes: bytes, header_row_index: int | None = 0) \
             -> tuple[DataFrame, DataFrame | None]:
         """
@@ -376,7 +228,201 @@
 
         with io.BytesIO() as output:
             with pandas.ExcelWriter(output, engine='xlsxwriter') as writer:
                 # Setting header and index to false makes the CSV convert to an XLSX as-is.
                 data_frame.to_excel(writer, sheet_name='Sheet1', header=False, index=False)
             xlsx_data = output.getvalue()
         return xlsx_data
+
+    @staticmethod
+    def csv_to_xls(file_data: bytes | str, delimiter: str = ",", newline: str = "\r\n") -> bytes:
+        """
+        Convert the bytes or string of a .csv file to .xls bytes.
+
+        :param file_data: The .csv bytes or string to convert.
+        :param delimiter: The delimiter character separating columns, with "," being the default.
+        :param newline: The newline character(s) separating rows, with "\r\n" being the default.
+        :return: The bytes of the new .xls file.
+        """
+        # Import the libraries we'll need locally since we won't be using them anywhere else in the class.
+        from xlwt import Workbook, Worksheet
+
+        # Create an Excel workbook along with a worksheet, which is where the data will be written.
+        workbook: Workbook = Workbook()
+        sheet: Worksheet = workbook.add_sheet("Sheet1")
+
+        # Make sure the file data is in a string format so that we can work with it.
+        formatted_data: str = bytes.decode(file_data, "utf-8") if isinstance(file_data, bytes) else file_data
+
+        # Write each row of the file to the .xls sheet.
+        rows: list[str] = formatted_data.split(newline)
+        for i, row in enumerate(rows):
+            values: list[str] = row.split(delimiter)
+            for j, value in enumerate(values):
+                sheet.write(i, j, value)
+
+        # Save the worksheet data to the byte buffer and return the bytes.
+        with io.BytesIO() as buffer:
+            workbook.save(buffer)
+            file_bytes: bytes = buffer.getvalue()
+        return file_bytes
+
+    # Deprecated functions:
+
+    # FR-46097 - Add write file request shorthand functions to FileUtil.
+    @staticmethod
+    def write_file(file_name: str, file_bytes: bytes, *, request_context: str | None = None) -> SapioWebhookResult:
+        """
+        DEPRECATED: Make use of CallbackUtil as of 24.5.
+
+        Send a file to the client.
+
+        The calling webhook must catch the WriteFileResult that the client will send back.
+
+        :param file_name: The name of the file.
+        :param file_bytes: The bytes of the file.
+        :param request_context: Context that will be returned to the webhook server in the client callback result.
+        :return: A SapioWebhookResult with the write request as its client callback request.
+        """
+        return SapioWebhookResult(True, client_callback_request=WriteFileRequest(file_bytes, file_name,
+                                                                                 request_context))
+
+    @staticmethod
+    def write_files(files: dict[str, bytes], *, request_context: str | None = None) -> SapioWebhookResult:
+        """
+        DEPRECATED: Make use of CallbackUtil as of 24.5.
+
+        Send a collection of files to the client.
+
+        The calling webhook must catch the MultiFileResult that the client will send back.
+
+        :param files: A dictionary of files names to file bytes.
+        :param request_context: Context that will be returned to the webhook server in the client callback result.
+        :return: A SapioWebhookResult with the write request as its client callback request.
+        """
+        return SapioWebhookResult(True, client_callback_request=MultiFileRequest(files, request_context))
+
+    @staticmethod
+    def request_file(context: SapioWebhookContext, title: str, exts: list[str] = None,
+                     *, request_context: str | None = None) \
+            -> tuple[SapioWebhookResult | None, str | None, bytes | None]:
+        """
+        DEPRECATED: Make use of CallbackUtil as of 24.5.
+
+        Request a single file from the user. This function handles the entire client callback interaction for the
+        requesting of the file, including if the user cancels the file upload prompt.
+
+        The first time this method is called in the course of an interaction with the client, it will return a webhook
+        result containing the client callback to request the file. The second time it is called, it will return the
+        file name and bytes from the callback result.
+
+        :param context: The current webhook context.
+        :param title: The title of the file prompt dialog.
+        :param exts: The allowable file extensions of the uploaded file. If blank, any file can be uploaded. Throws an
+            exception if an incorrect file extension is provided.
+        :param request_context: Context that will be returned to the webhook server in the client callback result.
+        :return: A tuple with the following elements.
+            0 - A webhook result that contains a file prompt if this is the first interaction with this request.
+            May also contain a result that will terminate the client interaction if the user canceled the prompt.
+            1 - The file name of the requested file if the user provided one.
+            2 - The file bytes of the requested file if the user provided one.
+        """
+        client_callback = context.client_callback_result
+        result_context: str | None = client_callback.callback_context_data if client_callback else None
+        # If the user cancels, terminate the interaction.
+        if client_callback is not None and client_callback.user_cancelled:
+            return SapioWebhookResult(True), None, None
+        # If no extensions were provided, use an empty list for the extensions instead.
+        if exts is None:
+            exts = []
+
+        # If the client callback isn't a FilePromptResult, then it's either None or some other callback result, meaning
+        # we need to send a new request. We may also send a new request if the client callback result is a
+        # FilePromptResult, but its callback context doesn't match the provided callback context, meaning it's a
+        # result from a different call to request_file.
+        is_file_result = isinstance(client_callback, FilePromptResult)
+        if not is_file_result or (is_file_result and result_context != request_context):
+            prompt = FilePromptRequest(dialog_title=title, file_extension=",".join(exts),
+                                       callback_context_data=request_context)
+            return SapioWebhookResult(True, client_callback_request=prompt), None, None
+
+        # Get the file from the result. Enforce that the provided data isn't empty, and that the file path ends in
+        # one of the allowed extensions.
+        # noinspection PyTypeChecker
+        result: FilePromptResult = client_callback
+        file_path: str | None = result.file_path
+        file_bytes: bytes | None = result.file_bytes
+        FileUtil.__verify_file(file_path, file_bytes, exts)
+        return None, file_path, file_bytes
+
+    @staticmethod
+    def request_files(context: SapioWebhookContext, title: str, exts: list[str] = None,
+                      *, request_context: str | None = None) \
+            -> tuple[SapioWebhookResult | None, dict[str, bytes] | None]:
+        """
+        DEPRECATED: Make use of CallbackUtil as of 24.5.
+
+        Request multiple files from the user. This function handles the entire client callback interaction for the
+        requesting of the files, including if the user cancels the file upload prompt.
+
+        The first time this method is called in the course of an interaction with the client, it will return a webhook
+        result containing the client callback to request the files. The second time it is called, it will return each
+        file name and bytes from the callback result.
+
+        :param context: The current webhook context.
+        :param title: The title of the file prompt dialog.
+        :param exts: The allowable file extensions of the uploaded file. If blank, any file can be uploaded. Throws an
+            exception if an incorrect file extension is provided.
+        :param request_context: Context that will be returned to the webhook server in the client callback result.
+        :return: A tuple with the following elements.
+            0 - A webhook result that contains a file prompt if this is the first interaction with this request.
+            May also contain a result that will terminate the client interaction if the user canceled the prompt.
+            1 - A dictionary that maps the file names to the file bytes for each provided file.
+        """
+        client_callback = context.client_callback_result
+        result_context: str | None = client_callback.callback_context_data if client_callback else None
+        # If the user cancels, terminate the interaction.
+        if client_callback is not None and client_callback.user_cancelled:
+            return SapioWebhookResult(True), None
+        # If no extensions were provided, use an empty list for the extensions instead.
+        if exts is None:
+            exts = []
+
+        # If the client callback isn't a MultiFilePromptResult, then it's either None or some other callback result,
+        # meaning we need to send a new request. We may also send a new request if the client callback result is a
+        # MultiFilePromptResult, but its callback context doesn't match the provided callback context, meaning it's a
+        # result from a different call to request_file.
+        is_file_result = isinstance(client_callback, MultiFilePromptResult)
+        if not is_file_result or (is_file_result and result_context != request_context):
+            prompt = MultiFilePromptRequest(dialog_title=title, file_extension=",".join(exts),
+                                            callback_context_data=request_context)
+            return SapioWebhookResult(True, client_callback_request=prompt), None
+
+        # Get the files from the result. Enforce that the provided data isn't empty, and that the file paths end in
+        # one of the allowed extensions.
+        # noinspection PyTypeChecker
+        result: MultiFilePromptResult = client_callback
+        for file_path, file_bytes in result.files.items():
+            FileUtil.__verify_file(file_path, file_bytes, exts)
+        return None, result.files
+
+    @staticmethod
+    def __verify_file(file_path: str, file_bytes: bytes, allowed_extensions: list[str]):
+        """
+        Verify that the provided file was read (i.e. the file path and file bytes aren't None or empty) and that it
+        has the correct file extension. Raises a user error exception if something about the file is incorrect.
+
+        :param file_path: The name of the file to verify.
+        :param file_bytes: The bytes of the file to verify.
+        :param allowed_extensions: The file extensions that the file path is allowed to have.
+        """
+        if file_path is None or len(file_path) == 0 or file_bytes is None or len(file_bytes) == 0:
+            raise SapioUserErrorException("Empty file provided or file unable to be read.")
+        if len(allowed_extensions) != 0:
+            matches: bool = False
+            for ext in allowed_extensions:
+                if file_path.endswith("." + ext):
+                    matches = True
+                    break
+            if matches is False:
+                raise SapioUserErrorException("Unsupported file type. Expecting the following extension(s): "
+                                              + (",".join(allowed_extensions)))
```

### Comparing `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/aliases.py` & `sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/aliases.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/exceptions.py` & `sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,24 +3,34 @@
     """
     A generic exception thrown by sapiopycommons methods. Typically caused by programmer error, but may also be from
     extremely edge case user errors. For expected user errors, use SapioUserErrorException.
     """
     pass
 
 
+# CommonsWebhookHandler catches this exception and returns "User Cancelled."
+class SapioUserCancelledException(SapioException):
+    """
+    An exception thrown when the user cancels a client callback.
+    """
+    pass
+
+
+# CommonsWebhookHandler catches this exception and returns the text to the user as display text in a webhook result.
 class SapioUserErrorException(SapioException):
     """
     An exception caused by user error (e.g. user provided a CSV when an XLSX was expected), which promises to return a
     user-friendly message explaining the error that should be displayed to the user. It is the responsibility of the
     programmer to catch any such exceptions and return the value in e.args[0] as text for the user to see (such as
     through the display text of a webhook result).
     """
     pass
 
 
+# CommonsWebhookHandler catches this exception and returns the text in a display_error client callback.
 class SapioCriticalErrorException(SapioException):
     """
     A critical exception caused by user error, which promises to return a user-friendly message explaining the error
     that should be displayed to the user. It is the responsibility of the programmer to catch any such exceptions and
     return the value in e.args[0] as text for the user to see (such as through a dialog form client callback request).
     """
     pass
```

### Comparing `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/popup_util.py` & `sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/popup_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,24 +13,29 @@
 
 
 # FR-46064 - Initial port of PyWebhookUtils to sapiopycommons.
 # FR-46097 - Greatly expand the options that PopupUtil provides. (Originally just had two OptionDialogRequest
 # and one FormEntryDialogRequest methods.)
 # CR-46332 - For any functions that use temporary data types, set the data type name, display name, and plural display
 # name in the form builder.
+# FR-46716 - Add comments noting that this class is deprecated in favor of CallbackUtil.
 class PopupUtil:
     """
+    DEPRECATED: Make use of CallbackUtil as of 24.5.
+
     Methods for creating boilerplate SapioWebhookResults with client callback requests to create popup dialogs.
     """
     @staticmethod
     def form_popup(title: str, msg: str, fields: list[AbstractVeloxFieldDefinition], values: FieldMap = None,
                    column_positions: dict[str, tuple[int, int]] = None, data_type: str = "Default",
                    *, display_name: str | None = None, plural_display_name: str | None = None,
                    request_context: str | None = None) -> SapioWebhookResult:
         """
+        DEPRECATED: Make use of CallbackUtil as of 24.5.
+
         Create a basic form entry dialog.
 
         The calling webhook must catch the FormEntryDialogResult that the client will send back.
 
         :param title: The title of the dialog.
         :param msg: The message to display at the top of the form.
         :param fields: The definitions of the fields to display in the form. Fields will be displayed in the order they
@@ -68,20 +73,22 @@
 
     @staticmethod
     def record_form_popup(context: SapioWebhookContext,
                           title: str, msg: str, fields: list[str], record: SapioRecord,
                           column_positions: dict[str, tuple[int, int]] = None, editable: bool | None = True,
                           *, request_context: str | None = None) -> SapioWebhookResult:
         """
+        DEPRECATED: Make use of CallbackUtil as of 24.5.
+
         Create a basic form dialog for a record with displayed fields from the record data type.
 
         Makes webservice calls to get the data field and type definitions of the given data type.
         The calling webhook must catch the FormEntryDialogResult that the client will send back.
 
-        :param context: The current webhook context
+        :param context: The current webhook context.
         :param title: The title of the dialog.
         :param msg: The message to display in the dialog.
         :param fields: The data field names of the fields from the record to display in the form. Fields will be
             displayed in the order they are provided in this list.
         :param record: The record to display the values of.
         :param column_positions: If a tuple is provided for a field name, alters that field's column position and column
             span. (Field order is still determined by the fields list.)
@@ -122,14 +129,16 @@
 
     @staticmethod
     def string_field_popup(title: str, msg: str, field_name: str, default_value: str | None = None,
                            max_length: int | None = None, editable: bool = True, data_type: str = "Default",
                            *, display_name: str | None = None, plural_display_name: str | None = None,
                            request_context: str | None = None, **kwargs) -> SapioWebhookResult:
         """
+        DEPRECATED: Make use of CallbackUtil as of 24.5.
+
         Create a form dialog with a single string field. May take additional parameters to be passed to the string field
         definition.
 
         The calling webhook must catch the FormEntryDialogResult that the client will send back.
 
         :param title: The title of the dialog.
         :param msg: The message to display in the dialog.
@@ -155,14 +164,16 @@
 
     @staticmethod
     def integer_field_popup(title: str, msg: str, field_name: str, default_value: int = None, min_value: int = -10000,
                             max_value: int = 10000, data_type: str = "Default", editable: bool = True,
                             *, display_name: str | None = None, plural_display_name: str | None = None,
                             request_context: str | None = None, **kwargs) -> SapioWebhookResult:
         """
+        DEPRECATED: Make use of CallbackUtil as of 24.5.
+
         Create a form dialog with a single integer field. May take additional parameters to be passed to the integer
         field definition.
 
         The calling webhook must catch the FormEntryDialogResult that the client will send back.
 
         :param title: The title of the dialog.
         :param msg: The message to display in the dialog.
@@ -191,14 +202,16 @@
     @staticmethod
     def double_field_popup(title: str, msg: str, field_name: str, default_value: float = None,
                            min_value: float = -10000000, max_value: float = 100000000,
                            data_type: str = "Default", editable: bool = True, *, display_name: str | None = None,
                            plural_display_name: str | None = None, request_context: str | None = None, **kwargs) \
             -> SapioWebhookResult:
         """
+        DEPRECATED: Make use of CallbackUtil as of 24.5.
+
         Create a form dialog with a single double field. May take additional parameters to be passed to the double
         field definition.
 
         The calling webhook must catch the FormEntryDialogResult that the client will send back.
 
         :param title: The title of the dialog.
         :param msg: The message to display in the dialog.
@@ -224,14 +237,16 @@
                                     plural_display_name=plural_display_name, request_context=request_context)
 
     @staticmethod
     def table_popup(title: str, msg: str, fields: list[AbstractVeloxFieldDefinition], values: list[FieldMap],
                     *, data_type: str = "Default", display_name: str | None = None,
                     plural_display_name: str | None = None, request_context: str | None = None) -> SapioWebhookResult:
         """
+        DEPRECATED: Make use of CallbackUtil as of 24.5.
+
         Create a basic table entry dialog.
 
         The calling webhook must catch the TableEntryDialogResult that the client will send back.
 
         :param title: The title of the dialog.
         :param msg: The message to display at the top of the form.
         :param fields: The definitions of the fields to display as table columns. Fields will be displayed in the order
@@ -258,14 +273,16 @@
         return SapioWebhookResult(True, client_callback_request=callback)
 
     @staticmethod
     def record_table_popup(context: SapioWebhookContext,
                            title: str, msg: str, fields: list[str], records: list[SapioRecord],
                            editable: bool | None = True, *, request_context: str | None = None) -> SapioWebhookResult:
         """
+        DEPRECATED: Make use of CallbackUtil as of 24.5.
+
         Create a table dialog for a list of record where the columns are specific fields from the record data type.
 
         Makes webservice calls to get the data field and type definitions of the given data type.
         The calling webhook must catch the TableEntryDialogResult that the client will send back.
 
         :param context: The current webhook context
         :param title: The title of the dialog.
@@ -309,14 +326,16 @@
         return SapioWebhookResult(True, client_callback_request=callback)
 
     @staticmethod
     def record_selection_popup(context: SapioWebhookContext,
                                msg: str, fields: list[str], records: list[SapioRecord], multi_select: bool = True,
                                *, request_context: str | None = None) -> SapioWebhookResult:
         """
+        DEPRECATED: Make use of CallbackUtil as of 24.5.
+
         Create a record selection dialog for a list of record where the columns are specific fields from the record data
         type.
 
         Makes webservice calls to get the data field and type definitions of the given data type.
         The calling webhook must catch the DataRecordSelectionResult that the client will send back.
 
         :param context: The current webhook context
@@ -356,14 +375,16 @@
                                               callback_context_data=request_context)
         return SapioWebhookResult(True, client_callback_request=callback)
 
     @staticmethod
     def list_popup(title: str, options: list[str], multi_select: bool = False,
                    *, request_context: str | None = None) -> SapioWebhookResult:
         """
+        DEPRECATED: Make use of CallbackUtil as of 24.5.
+
         Create a list dialog with the given options for the user to choose from.
 
         The calling webhook must catch the ListDialogResult that the client will send back.
 
         :param title: The title of the dialog.
         :param options: The list options that the user has to choose from.
         :param multi_select: Whether the user is able to select multiple options from the list.
@@ -374,14 +395,16 @@
                                      callback_context_data=request_context)
         return SapioWebhookResult(True, client_callback_request=callback)
 
     @staticmethod
     def option_popup(title: str, msg: str, options: list[str], default_option: int = 0, user_can_cancel: bool = False,
                      *, request_context: str | None = None) -> SapioWebhookResult:
         """
+        DEPRECATED: Make use of CallbackUtil as of 24.5.
+
         Create an option dialog with the given options for the user to choose from.
 
         The calling webhook must catch the OptionDialogResult that the client will send back.
 
         :param title: The title of the dialog.
         :param msg: The message to display in the dialog.
         :param options: The button options that the user has to choose from.
@@ -396,14 +419,16 @@
                                        callback_context_data=request_context)
         return SapioWebhookResult(True, client_callback_request=callback)
 
     @staticmethod
     def ok_popup(title: str, msg: str, user_can_cancel: bool = False, *, request_context: str | None = None) \
             -> SapioWebhookResult:
         """
+        DEPRECATED: Make use of CallbackUtil as of 24.5.
+
         Create an option dialog where the only option is "OK".
 
         The calling webhook must catch the OptionDialogResult that the client will send back.
 
         :param title: The title of the dialog.
         :param msg: The message to display in the dialog.
         :param user_can_cancel: True if the user is able to click the X to close the dialog, returning
@@ -414,14 +439,16 @@
         """
         return PopupUtil.option_popup(title, msg, ["OK"], 0, user_can_cancel, request_context=request_context)
 
     @staticmethod
     def yes_no_popup(title: str, msg: str, default_yes: bool = True, user_can_cancel: bool = False,
                      *, request_context: str | None = None) -> SapioWebhookResult:
         """
+        DEPRECATED: Make use of CallbackUtil as of 24.5.
+
         Create an option dialog where the only options are "Yes" and "No".
 
         The calling webhook must catch the OptionDialogResult that the client will send back.
 
         :param title: The title of the dialog.
         :param msg: The message to display in the dialog.
         :param default_yes: If true, "Yes" is the default choice. Otherwise, the default choice is "No".
@@ -435,26 +462,32 @@
                                       request_context=request_context)
 
     # FR-46097 - Deprecating the three original functions for ones with briefer names. Functionality is unchanged.
     @staticmethod
     def display_form_popup(title: str, field_name: str, msg: str, data_type: str = "Popup",
                            request_context: str | None = None) -> SapioWebhookResult:
         """
+        DEPRECATED: Make use of CallbackUtil as of 24.5.
+
         Deprecated for PopupUtil.text_field_popup.
         """
         return PopupUtil.string_field_popup(title, "", field_name, msg, len(msg), False, data_type,
                                             request_context=request_context, auto_size=True)
 
     @staticmethod
     def display_option_popup(title: str, msg: str, options: list[str], user_can_cancel: bool = False,
                              request_context: str | None = None) -> SapioWebhookResult:
         """
+        DEPRECATED: Make use of CallbackUtil as of 24.5.
+
         Deprecated for PopupUtil.option_popup.
         """
         return PopupUtil.option_popup(title, msg, options, 0, user_can_cancel, request_context=request_context)
 
     @staticmethod
     def display_ok_popup(title: str, msg: str, request_context: str | None = None) -> SapioWebhookResult:
         """
+        DEPRECATED: Make use of CallbackUtil as of 24.5.
+
         Deprecated for PopupUtil.ok_popup.
         """
         return PopupUtil.ok_popup(title, msg, False, request_context=request_context)
```

### Comparing `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/storage_util.py` & `sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/storage_util.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/time_util.py` & `sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/time_util.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/processtracking/endpoints.py` & `sapiopycommons-32.0.0.24.5/src/sapiopycommons/processtracking/endpoints.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+from sapiopylib.rest.User import SapioUser
 from sapiopylib.rest.pojo.webhook.WebhookContext import SapioWebhookContext
 
 from sapiopycommons.general.aliases import RecordIdentifier, AliasUtil, ExperimentIdentifier
 
 
 class ProcessTracking:
     @staticmethod
-    def assign_to_process(context: SapioWebhookContext, data_type: str, records: list[RecordIdentifier],
+    def assign_to_process(context: SapioWebhookContext | SapioUser, data_type: str, records: list[RecordIdentifier],
                           process_name: str, step_number: int | None = None, branch_id: int | None = None,
                           request: RecordIdentifier | None = None) -> None:
         """
         Assign the given tracked records to a new process at the specified step, settings its status to "Ready for -"
         at that step.
         Synonymous with what occurs during request creation or when using the assign to process button.
 
-        :param context: The current webhook context.
+        :param context: The current webhook context or a user object to send requests from.
         :param data_type: The data type of the tracked records.
         :param records: A list of the tracked records.
         :param process_name: The name of the process that the tracked records should start at.
         :param step_number: The step number that the tracked records should start at. If not provided, assumes step
             number 1.
         :param branch_id: The branch ID of the above step. Only necessary to provide if multiple steps in the process
             share the same step number.
@@ -29,124 +30,130 @@
             "data-type-name": data_type,
             "record-ids": AliasUtil.to_record_ids(records),
             "process-name": process_name,
             "step-number": step_number,
             "branch-id": branch_id,
             "request-record-id": AliasUtil.to_record_ids([request])[0] if request is not None else None
         }
-        response = context.user.post(sub_path, payload=payload)
-        context.user.raise_for_status(response)
+        user: SapioUser = context if isinstance(context, SapioUser) else context.user
+        response = user.post(sub_path, payload=payload)
+        user.raise_for_status(response)
 
     @staticmethod
-    def begin_protocol(context: SapioWebhookContext, data_type: str, records: list[RecordIdentifier],
+    def begin_protocol(context: SapioWebhookContext | SapioUser, data_type: str, records: list[RecordIdentifier],
                        experiment: ExperimentIdentifier) -> None:
         """
         Begin the assigned processes of the given tracked records as the given experiment. This sets the status of the
         tracked records from "Ready for -" to "In Process -" for their current step.
         Synonymous with what occurs when starting a process step in the system.
 
-        :param context: The current webhook context.
+        :param context: The current webhook context or a user object to send requests from.
         :param data_type: The data type of the tracked records.
         :param records: A list of the tracked records.
         :param experiment: The experiment that the tracked records are beginning the process for. This must be the next
             step in the current process of the tracked records.
         """
         sub_path = '/ext/process-tracking/begin-protocol'
         payload = {
             "data-type-name": data_type,
             "record-ids": AliasUtil.to_record_ids(records),
             "experiment-id": AliasUtil.to_notebook_id(experiment),
         }
-        response = context.user.post(sub_path, payload=payload)
-        context.user.raise_for_status(response)
+        user: SapioUser = context if isinstance(context, SapioUser) else context.user
+        response = user.post(sub_path, payload=payload)
+        user.raise_for_status(response)
 
     @staticmethod
-    def complete_protocol(context: SapioWebhookContext, data_type: str, records: list[RecordIdentifier],
+    def complete_protocol(context: SapioWebhookContext | SapioUser, data_type: str, records: list[RecordIdentifier],
                           experiment: ExperimentIdentifier) -> None:
         """
         Complete the current step that the given tracked records are at given the experiment.
         Moves the status to "Ready for -" for the next step in the process, or "Completed -" if this was the last
         step.
         Moves the status to "Failed -" if the failed flag for the tracked record is true.
         Moves the assigned process down to the descendant sample(s) if both samples are provided in the records list.
         Synonymous with what occurs when completing an experiment in the system.
 
-        :param context: The current webhook context.
+        :param context: The current webhook context or a user object to send requests from.
         :param data_type: The data type of the tracked records.
         :param records: A list of the tracked records.
         :param experiment: The experiment that the tracked records are currently in and completing.
         """
         sub_path = '/ext/process-tracking/complete-protocol'
         payload = {
             "data-type-name": data_type,
             "record-ids": AliasUtil.to_record_ids(records),
             "experiment-id": AliasUtil.to_notebook_id(experiment),
         }
-        response = context.user.post(sub_path, payload=payload)
-        context.user.raise_for_status(response)
+        user: SapioUser = context if isinstance(context, SapioUser) else context.user
+        response = user.post(sub_path, payload=payload)
+        user.raise_for_status(response)
 
     @staticmethod
-    def fail(context: SapioWebhookContext, data_type: str, records: list[RecordIdentifier],
+    def fail(context: SapioWebhookContext | SapioUser, data_type: str, records: list[RecordIdentifier],
              experiment: ExperimentIdentifier) -> None:
         """
         Fail the assigned processes of the given tracked records, changing their statuses to "Failed -". The tracked
         records must be "In Process -" for the given step.
         Synonymous with what occurs when failing a sample due to a QC failure in a process in the system.
 
-        :param context: The current webhook context.
+        :param context: The current webhook context or a user object to send requests from.
         :param data_type: The data type of the tracked records.
         :param records: A list of the tracked records.
         :param experiment: The experiment that the tracked records are currently in.
         """
         sub_path = '/ext/process-tracking/fail'
         payload = {
             "data-type-name": data_type,
             "record-ids": AliasUtil.to_record_ids(records),
             "experiment-id": AliasUtil.to_notebook_id(experiment),
         }
-        response = context.user.post(sub_path, payload=payload)
-        context.user.raise_for_status(response)
+        user: SapioUser = context if isinstance(context, SapioUser) else context.user
+        response = user.post(sub_path, payload=payload)
+        user.raise_for_status(response)
 
     @staticmethod
-    def promote_to_next_by_experiment(context: SapioWebhookContext, data_type: str, records: list[RecordIdentifier],
-                                      experiment: ExperimentIdentifier) -> None:
+    def promote_to_next_by_experiment(context: SapioWebhookContext | SapioUser, data_type: str,
+                                      records: list[RecordIdentifier], experiment: ExperimentIdentifier) -> None:
         """
         Promote the status of the given tracked records to the next status in their process using an experiment.
         If the tracked records currently have a status of "Ready for -", then providing an experiment of the template
         they are ready for will move their status to "In Process -" for the experiment.
         If the tracked records currently have a status of "In Process -", then providing their current experiment
         will move their status to "Ready for -" for the next step in the process, or "Completed -" if this was the
         last step.
 
-        :param context: The current webhook context.
+        :param context: The current webhook context or a user object to send requests from.
         :param data_type: The data type of the tracked records.
         :param records: A list of the tracked records.
         :param experiment: The experiment that the tracked records are currently in.
         """
         sub_path = '/ext/process-tracking/promote-status-to-next'
         payload = {
             "data-type-name": data_type,
             "record-ids": AliasUtil.to_record_ids(records),
             "experiment-id": AliasUtil.to_notebook_id(experiment),
         }
-        response = context.user.post(sub_path, payload=payload)
-        context.user.raise_for_status(response)
+        user: SapioUser = context if isinstance(context, SapioUser) else context.user
+        response = user.post(sub_path, payload=payload)
+        user.raise_for_status(response)
 
     @staticmethod
-    def promote_to_next_by_step(context: SapioWebhookContext, data_type: str, records: list[RecordIdentifier],
-                                process_name: str, step_number: int, branch_id: int | None = None) -> None:
+    def promote_to_next_by_step(context: SapioWebhookContext | SapioUser, data_type: str,
+                                records: list[RecordIdentifier], process_name: str, step_number: int,
+                                branch_id: int | None = None) -> None:
         """
         Promote the status of the given tracked records to the next status in their process using step info.
         If the tracked records currently have a status of "Ready for -", then providing the step info for their current
         step will move their status to "In Process -" for that step.
         If the tracked records currently have a status of "In Process -", then providing the step info for their current
         step will move their status to "Ready for -" for the next step in the process, or "Completed -" if this was the
         last step.
 
-        :param context: The current webhook context.
+        :param context: The current webhook context or a user object to send requests from.
         :param data_type: The data type of the tracked records.
         :param records: A list of the tracked records.
         :param process_name: The name of the process that the tracked records are currently in.
         :param step_number: The step number that the tracked records are currently in.
         :param branch_id: The branch ID of the above step. Only necessary to provide if multiple steps in the process
             share the same step number.
         """
@@ -156,28 +163,30 @@
             "record-ids": AliasUtil.to_record_ids(records),
             "current-process-status": {
                 "process-name": process_name,
                 "step-number": step_number,
                 "branch-id": branch_id
             }
         }
-        response = context.user.post(sub_path, payload=payload)
-        context.user.raise_for_status(response)
+        user: SapioUser = context if isinstance(context, SapioUser) else context.user
+        response = user.post(sub_path, payload=payload)
+        user.raise_for_status(response)
 
     @staticmethod
-    def reprocess(context: SapioWebhookContext, records: list[RecordIdentifier]) -> None:
+    def reprocess(context: SapioWebhookContext | SapioUser, records: list[RecordIdentifier]) -> None:
         """
         Reprocess tracked records to a previous step in their process. Reprocessing is controlled by ReturnPoint records
         which are children of the AssignedProcess on the tracked records. Creates a new AssignedProcess record for the
         effected tracked records. Any existing AssignedProcess records are untouched.
         Synonymous with what occurs when reprocessing records to a previous step due to QC failures in a process in the
         system.
 
-        :param context: The current webhook context.
+        :param context: The current webhook context or a user object to send requests from.
         :param records: A list of ReturnPoint records to reprocess to.
         """
         sub_path = '/ext/process-tracking/reprocess'
         payload = {
             "record-ids": AliasUtil.to_record_ids(records)
         }
-        response = context.user.post(sub_path, payload=payload)
-        context.user.raise_for_status(response)
+        user: SapioUser = context if isinstance(context, SapioUser) else context.user
+        response = user.post(sub_path, payload=payload)
+        user.raise_for_status(response)
```

### Comparing `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/recordmodel/record_handler.py` & `sapiopycommons-32.0.0.24.5/src/sapiopycommons/recordmodel/record_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 from collections.abc import Iterable
 from typing import Any
 
 from sapiopylib.rest.DataRecordManagerService import DataRecordManager
+from sapiopylib.rest.User import SapioUser
 from sapiopylib.rest.pojo.DataRecord import DataRecord
 from sapiopylib.rest.pojo.DataRecordPaging import DataRecordPojoPageCriteria
 from sapiopylib.rest.pojo.webhook.WebhookContext import SapioWebhookContext
+from sapiopylib.rest.utils.autopaging import QueryDataRecordsAutoPager, QueryDataRecordByIdListAutoPager, \
+    QueryAllRecordsOfTypeAutoPager
 from sapiopylib.rest.utils.recordmodel.PyRecordModel import PyRecordModel
 from sapiopylib.rest.utils.recordmodel.RecordModelManager import RecordModelManager, RecordModelInstanceManager, \
     RecordModelRelationshipManager
-from sapiopylib.rest.utils.recordmodel.RecordModelWrapper import WrappedType
-from sapiopylib.rest.utils.recordmodel.RelationshipPath import RelationshipPath, RelationshipPathDir
+from sapiopylib.rest.utils.recordmodel.RecordModelWrapper import WrappedType, WrappedRecordModel
+from sapiopylib.rest.utils.recordmodel.RelationshipPath import RelationshipPath, RelationshipNode, \
+    RelationshipNodeType
 
 from sapiopycommons.general.aliases import RecordModel, SapioRecord, FieldMap
 from sapiopycommons.general.custom_report_util import CustomReportUtil
 from sapiopycommons.general.exceptions import SapioException
 
 
 # FR-46064 - Initial port of PyWebhookUtils to sapiopycommons.
 class RecordHandler:
     """
     A collection of shorthand methods for dealing with the various record managers.
     """
-    __context: SapioWebhookContext
+    user: SapioUser
     dr_man: DataRecordManager
     rec_man: RecordModelManager
     inst_man: RecordModelInstanceManager
     rel_man: RecordModelRelationshipManager
 
-    def __init__(self, context: SapioWebhookContext):
+    def __init__(self, context: SapioWebhookContext | SapioUser):
         """
-        :param context: The current webhook context.
+        :param context: The current webhook context or a user object to send requests from.
         """
-        self.__context = context
-        self.dr_man = context.data_record_manager
-        self.rec_man = RecordModelManager(context.user)
+        self.user = context if isinstance(context, SapioUser) else context.user
+        self.dr_man = DataRecordManager(self.user)
+        self.rec_man = RecordModelManager(self.user)
         self.inst_man = self.rec_man.instance_manager
         self.rel_man = self.rec_man.relationship_manager
 
     def wrap_model(self, record: DataRecord, wrapper_type: type[WrappedType]) -> WrappedType:
         """
         Shorthand for adding a single data record as a record model.
 
@@ -84,16 +88,17 @@
         :param value_list: The values of the field to query on.
         :param paging_criteria: The paging criteria to start the query with.
         :param page_limit: The maximum number of pages to query from the starting criteria. If None, exhausts all
             possible pages.
         :return: The record models for the queried records and the final paging criteria.
         """
         dt: str = wrapper_type.get_wrapper_data_type_name()
-        records, paging_criteria = self.__exhaust_query_pages(dt, field, list(value_list), paging_criteria, page_limit)
-        return self.wrap_models(records, wrapper_type), paging_criteria
+        pager = QueryDataRecordsAutoPager(dt, field, list(value_list), self.user, paging_criteria)
+        pager.max_page = page_limit
+        return self.wrap_models(pager.get_all_at_once(), wrapper_type), pager.next_page_criteria
 
     def query_models_by_id(self, wrapper_type: type[WrappedType], ids: Iterable[int],
                            page_limit: int | None = None) -> list[WrappedType]:
         """
         Shorthand for using the data record manager to query for a list of data records by record ID
         and then converting the results into a list of record models.
 
@@ -116,16 +121,17 @@
         :param ids: The list of record IDs to query.
         :param paging_criteria: The paging criteria to start the query with.
         :param page_limit: The maximum number of pages to query from the starting criteria. If None, exhausts all
             possible pages.
         :return: The record models for the queried records and the final paging criteria.
         """
         dt: str = wrapper_type.get_wrapper_data_type_name()
-        records, paging_criteria = self.__exhaust_query_id_pages(dt, list(ids), paging_criteria, page_limit)
-        return self.wrap_models(records, wrapper_type), paging_criteria
+        pager = QueryDataRecordByIdListAutoPager(dt, list(ids), self.user, paging_criteria)
+        pager.max_page = page_limit
+        return self.wrap_models(pager.get_all_at_once(), wrapper_type), pager.next_page_criteria
 
     def query_all_models(self, wrapper_type: type[WrappedType], page_limit: int | None = None) -> list[WrappedType]:
         """
         Shorthand for using the data record manager to query for all data records of a given type
         and then converting the results into a list of record models.
 
         :param wrapper_type: The record model wrapper to use.
@@ -145,16 +151,17 @@
         :param wrapper_type: The record model wrapper to use.
         :param paging_criteria: The paging criteria to start the query with.
         :param page_limit: The maximum number of pages to query from the starting criteria. If None, exhausts all
             possible pages.
         :return: The record models for the queried records and the final paging criteria.
         """
         dt: str = wrapper_type.get_wrapper_data_type_name()
-        records, paging_criteria = self.__exhaust_query_all_pages(dt, paging_criteria, page_limit)
-        return self.wrap_models(records, wrapper_type), paging_criteria
+        pager = QueryAllRecordsOfTypeAutoPager(dt, self.user, paging_criteria)
+        pager.max_page = page_limit
+        return self.wrap_models(pager.get_all_at_once(), wrapper_type), pager.next_page_criteria
 
     def query_models_by_report(self, wrapper_type: type[WrappedType],
                                report_name: str,
                                filters: dict[str, Iterable[Any]] | None = None,
                                page_limit: int | None = None) -> list[WrappedType]:
         """
         Run a system report that contains a RecordId column and query for the records with those IDs.
@@ -165,15 +172,15 @@
         :param wrapper_type: The record model wrapper to use.
         :param report_name: The name of the system report to run.
         :param filters: If provided, filter the results of the report using the given mapping of headers to values to
             filter on. This filtering is done before the records are queried.
         :param page_limit: The maximum number of pages to query. If None, exhausts all possible pages.
         :return: The record models for the queried records.
         """
-        results: list[dict[str, Any]] = CustomReportUtil.run_system_report(self.__context, report_name, filters, page_limit)
+        results: list[dict[str, Any]] = CustomReportUtil.run_system_report(self.user, report_name, filters, page_limit)
         # Using the bracket operators because we want to throw an exception if RecordId doesn't exist in the report.
         ids: list[int] = [row["RecordId"] for row in results]
         return self.query_models_by_id(wrapper_type, ids)
 
     def add_model(self, wrapper_type: type[WrappedType]) -> WrappedType:
         """
         Shorthand for using the instance manager to add a new record model of the given type.
@@ -388,14 +395,96 @@
         by_children: dict[WrappedType, list[RecordModel]] = {}
         for record, children in to_children.items():
             for child in children:
                 by_children.setdefault(child, []).append(record)
         return by_children
 
     @staticmethod
+    def map_to_forward_side_link(models: Iterable[WrappedRecordModel], field_name: str,
+                                 side_link_type: type[WrappedType]) -> dict[WrappedRecordModel, WrappedType]:
+        """
+        Map a list of record models to their forward side link. The forward side link must already be loaded.
+
+        :param models: A list of record models.
+        :param field_name: The field name on the record models where the side link is located.
+        :param side_link_type: The record model wrapper of the forward side link.
+        :return: A dict[ModelType, SlideLink]. If an input model doesn't have a forward side link of the given type,
+            then it will map to None.
+        """
+        return_dict: dict[WrappedRecordModel, WrappedType] = {}
+        for model in models:
+            return_dict[model] = model.get_forward_side_link(field_name, side_link_type)
+        return return_dict
+
+    @staticmethod
+    def map_by_forward_side_link(models: Iterable[WrappedRecordModel], field_name: str,
+                                 side_link_type: type[WrappedType]) -> dict[WrappedType, list[WrappedRecordModel]]:
+        """
+        Take a list of record models and map them by their forward side link. Essentially an inversion of
+        map_to_forward_side_link. Input models that share a forward side link will end up in the same list.
+        The forward side link must already be loaded.
+
+        :param models: A list of record models.
+        :param field_name: The field name on the record models where the side link is located.
+        :param side_link_type: The record model wrapper of the forward side links.
+        :return: A dict[SideLink, list[ModelType]]. If an input model doesn't have a forward side link of the given type
+            pointing to it, then it will not be in the resulting dictionary.
+        """
+        to_side_link: dict[RecordModel, WrappedType] = RecordHandler\
+            .map_to_forward_side_link(models, field_name, side_link_type)
+        by_side_link: dict[WrappedType, list[RecordModel]] = {}
+        for record, side_link in to_side_link.items():
+            if side_link is None:
+                continue
+            by_side_link.setdefault(side_link, []).append(record)
+        return by_side_link
+
+    @staticmethod
+    def map_to_reverse_side_links(models: Iterable[WrappedRecordModel], field_name: str,
+                                  side_link_type: type[WrappedType]) -> dict[RecordModel, list[WrappedRecordModel]]:
+        """
+        Map a list of record models to a list reverse side links of a given type. The reverse side links must already
+        be loaded.
+
+        :param models: A list of record models.
+        :param field_name: The field name on the side linked model where the side link to the given record models is
+            located.
+        :param side_link_type: The record model wrapper of the reverse side links.
+        :return: A dict[ModelType, list[SideLink]]. If an input model doesn't have reverse side links of the given type,
+            then it will map to an empty list.
+        """
+        return_dict: dict[WrappedRecordModel, list[WrappedType]] = {}
+        for model in models:
+            return_dict[model] = model.get_reverse_side_link(field_name, side_link_type)
+        return return_dict
+
+    @staticmethod
+    def map_by_reverse_side_links(models: Iterable[WrappedRecordModel], field_name: str,
+                                  side_link_type: type[WrappedType]) -> dict[WrappedType, list[WrappedRecordModel]]:
+        """
+        Take a list of record models and map them by their reverse side links. Essentially an inversion of
+        map_to_reverse_side_links. Input models that share a reverse side link will end up in the same list.
+        The reverse side links must already be loaded.
+
+        :param models: A list of record models.
+        :param field_name: The field name on the side linked model where the side link to the given record models is
+            located.
+        :param side_link_type: The record model wrapper of the reverse side links.
+        :return: A dict[SideLink, list[ModelType]]. If an input model doesn't have reverse side links of the given type
+            pointing to it, then it will not be in the resulting dictionary.
+        """
+        to_side_links: dict[RecordModel, list[WrappedType]] = RecordHandler\
+            .map_to_reverse_side_links(models, field_name, side_link_type)
+        by_side_links: dict[WrappedType, list[RecordModel]] = {}
+        for record, side_links in to_side_links.items():
+            for side_link in side_links:
+                by_side_links.setdefault(side_link, []).append(record)
+        return by_side_links
+
+    @staticmethod
     def map_by_id(models: Iterable[SapioRecord]) -> dict[int, SapioRecord]:
         """
         Map the given records their record IDs.
 
         :param models: The records to map.
         :return: A dict mapping the record ID to each record.
         """
@@ -514,70 +603,82 @@
                 raise SapioException(f"Length of \"{field_name}\" values does not match the existing fields length.")
             for field, value in zip(existing_fields, values):
                 field.update({field_name: value})
             return existing_fields
         # Otherwise, create a new fields map list.
         return [{field_name: value} for value in values]
 
-    # FR-46155: Update relationship path traversing functions to be non-const and take in a wrapper type so that the
+    # FR-46155: Update relationship path traversing functions to be non-static and take in a wrapper type so that the
     # output can be wrapped instead of requiring the user to wrap the output.
     def get_linear_path(self, models: Iterable[RecordModel], path: RelationshipPath, wrapper_type: type[WrappedType]) \
             -> dict[RecordModel, WrappedType | None]:
         """
         Given a relationship path, travel the path starting from the input models. Returns the record at the end of the
         path, if any. The hierarchy must be linear (1:1 relationship between data types at every step) and the
         relationship path must already be loaded.
 
+        Currently, the relationship path may only contain parent/child nodes.
+
         :param models: A list of record models.
         :param path: The relationship path to follow.
         :param wrapper_type: The record model wrapper to use.
         :return: Each record model mapped to the record at the end of the path starting from itself. If the end of the
             path couldn't be reached, the record will map to None.
         """
         ret_dict: dict[RecordModel, WrappedType | None] = {}
-        path: list[tuple[RelationshipPathDir, str]] = path.path
+        # PR-46832: Update path traversal to account for changes to RelationshipPath in Sapiopylib.
+        path: list[RelationshipNode] = path.path
         for model in models:
             current: PyRecordModel = model if isinstance(model, PyRecordModel) else model.backing_model
-            for direction, datatype in path:
+            for node in path:
+                direction = node.direction
                 if current is None:
                     break
-                if direction == RelationshipPathDir.CHILD:
-                    current = current.get_child_of_type(datatype)
-                elif direction == RelationshipPathDir.PARENT:
-                    current = current.get_parent_of_type(datatype)
+                if direction == RelationshipNodeType.CHILD:
+                    current = current.get_child_of_type(node.data_type_name)
+                elif direction == RelationshipNodeType.PARENT:
+                    current = current.get_parent_of_type(node.data_type_name)
+                else:
+                    raise SapioException("Unsupported path direction.")
             ret_dict.update({model: self.inst_man.wrap(current, wrapper_type) if current else None})
         return ret_dict
 
     def get_branching_path(self, models: Iterable[RecordModel], path: RelationshipPath,
                            wrapper_type: type[WrappedType]) -> dict[RecordModel, list[WrappedType]]:
         """
         Given a relationship path, travel the path starting from the input models. Returns the record at the end of the
         path, if any. The hierarchy may be non-linear (1:Many relationships between data types are allowed) and the
         relationship path must already be loaded.
 
+        Currently, the relationship path may only contain parent/child nodes.
+
         :param models: A list of record models.
         :param path: The relationship path to follow.
         :param wrapper_type: The record model wrapper to use.
         :return: Each record model mapped to the records at the end of the path starting from itself. If the end of the
             path couldn't be reached, the record will map to an empty list.
         """
         ret_dict: dict[RecordModel, list[WrappedType]] = {}
-        path: list[tuple[RelationshipPathDir, str]] = path.path
+        # PR-46832: Update path traversal to account for changes to RelationshipPath in Sapiopylib.
+        path: list[RelationshipNode] = path.path
         for model in models:
             current_search: set[PyRecordModel] = {model if isinstance(model, PyRecordModel) else model.backing_model}
             next_search: set[PyRecordModel] = set()
             # Exhaust the records at each step in the path, then use those records for the next step.
-            for direction, datatype in path:
+            for node in path:
+                direction = node.direction
                 if len(current_search) == 0:
                     break
                 for search in current_search:
-                    if direction == RelationshipPathDir.CHILD:
-                        next_search.update(search.get_children_of_type(datatype))
-                    elif direction == RelationshipPathDir.PARENT:
-                        next_search.update(search.get_parents_of_type(datatype))
+                    if direction == RelationshipNodeType.CHILD:
+                        next_search.update(search.get_children_of_type(node.data_type_name))
+                    elif direction == RelationshipNodeType.PARENT:
+                        next_search.update(search.get_parents_of_type(node.data_type_name))
+                    else:
+                        raise SapioException("Unsupported path direction.")
                 current_search = next_search
                 next_search = set()
             ret_dict.update({model: self.inst_man.wrap_list(list(current_search), wrapper_type)})
         return ret_dict
 
     # FR-46155: Create a relationship traversing function that returns a single function at the end of the path like
     # get_linear_path but can handle branching paths in the middle of the search like get_branching_path.
@@ -588,71 +689,40 @@
         path, if any. The hierarchy may be non-linear (1:Many relationships between data types are allowed) and the
         relationship path must already be loaded.
 
         The path is "flattened" by only following the first record at each step. Useful for traversing 1-to-Many-to-1
         relationships (e.g. a sample with is aliquoted to a number of samples, then those aliquots are pooled back
         together into a single sample).
 
+        Currently, the relationship path may only contain parent/child nodes.
+
         :param models: A list of record models.
         :param path: The relationship path to follow.
         :param wrapper_type: The record model wrapper to use.
         :return: Each record model mapped to the record at the end of the path starting from itself. If the end of the
             path couldn't be reached, the record will map to None.
         """
         ret_dict: dict[RecordModel, WrappedType | None] = {}
-        path: list[tuple[RelationshipPathDir, str]] = path.path
+        # PR-46832: Update path traversal to account for changes to RelationshipPath in Sapiopylib.
+        path: list[RelationshipNode] = path.path
         for model in models:
             current: list[PyRecordModel] = [model if isinstance(model, PyRecordModel) else model.backing_model]
-            for direction, datatype in path:
+            for node in path:
+                direction = node.direction
                 if len(current) == 0:
                     break
-                if direction == RelationshipPathDir.CHILD:
-                    current = current[0].get_children_of_type(datatype)
-                elif direction == RelationshipPathDir.PARENT:
-                    current = current[0].get_parents_of_type(datatype)
+                if direction == RelationshipNodeType.CHILD:
+                    current = current[0].get_children_of_type(node.data_type_name)
+                elif direction == RelationshipNodeType.PARENT:
+                    current = current[0].get_parents_of_type(node.data_type_name)
+                else:
+                    raise SapioException("Unsupported path direction.")
             ret_dict.update({model: self.inst_man.wrap(current[0], wrapper_type) if current else None})
         return ret_dict
 
     def __exhaust_query_pages(self, data_type_name: str, field: str, value_list: list[Any],
                               paging_criteria: DataRecordPojoPageCriteria | None,
                               page_limit: int | None) \
             -> tuple[list[DataRecord], DataRecordPojoPageCriteria | None]:
-        has_next_page: bool = True
-        records: list[DataRecord] = []
-        cur_page: int = 1
-        while has_next_page and (not page_limit or cur_page < page_limit):
-            page_result = self.dr_man.query_data_records(data_type_name, field, value_list, paging_criteria)
-            paging_criteria = page_result.next_page_criteria
-            has_next_page = page_result.is_next_page_available
-            records.extend(page_result.result_list)
-            cur_page += 1
-        return records, paging_criteria
-
-    def __exhaust_query_id_pages(self, data_type_name: str, id_list: list[int],
-                                 paging_criteria: DataRecordPojoPageCriteria | None,
-                                 page_limit: int | None) \
-            -> tuple[list[DataRecord], DataRecordPojoPageCriteria | None]:
-        has_next_page: bool = True
-        records: list[DataRecord] = []
-        cur_page: int = 1
-        while has_next_page and (not page_limit or cur_page < page_limit):
-            page_result = self.dr_man.query_data_records_by_id(data_type_name, id_list, paging_criteria)
-            paging_criteria = page_result.next_page_criteria
-            has_next_page = page_result.is_next_page_available
-            records.extend(page_result.result_list)
-            cur_page += 1
-        return records, paging_criteria
-
-    def __exhaust_query_all_pages(self, data_type_name: str,
-                                  paging_criteria: DataRecordPojoPageCriteria | None,
-                                  page_limit: int | None) \
-            -> tuple[list[DataRecord], DataRecordPojoPageCriteria | None]:
-        has_next_page: bool = True
-        records: list[DataRecord] = []
-        cur_page: int = 1
-        while has_next_page and (not page_limit or cur_page < page_limit):
-            page_result = self.dr_man.query_all_records_of_type(data_type_name, paging_criteria)
-            paging_criteria = page_result.next_page_criteria
-            has_next_page = page_result.is_next_page_available
-            records.extend(page_result.result_list)
-            cur_page += 1
-        return records, paging_criteria
+        pager = QueryDataRecordsAutoPager(data_type_name, field, value_list, self.user, paging_criteria)
+        pager.max_page = page_limit
+        return pager.get_all_at_once(), pager.next_page_criteria
```

### Comparing `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/rules/eln_rule_handler.py` & `sapiopycommons-32.0.0.24.5/src/sapiopycommons/rules/eln_rule_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -100,14 +100,28 @@
                         data_type = "ELNSampleDetail"
                     for field_map in result.field_map_list:
                         rec_id: int = field_map.get("RecordId")
                         self.__field_maps.setdefault(data_type, {}).update({rec_id: field_map})
                         entry_dict.setdefault(data_type, {}).update({rec_id: field_map})
             self.__entry_to_field_maps.update({entry: entry_dict})
 
+    def get_entry_names(self) -> list[str]:
+        """
+        :return: A list of the entry names that may be used with the get_records and get_models functions. These are the
+            entries from the experiment that the records in the rule context originate from.
+        """
+        return list(self.__entry_to_records.keys())
+
+    def get_field_maps_entry_names(self) -> list[str]:
+        """
+        :return: A list of the entry names that may be used with the get_field_maps function. These are the
+            entries from the experiment that the field maps in the rule context originate from.
+        """
+        return list(self.__entry_to_field_maps.keys())
+
     def get_records(self, data_type: str, entry: str | None = None) -> list[DataRecord]:
         """
         Get records from the cached context with the given data type. Capable of being filtered to searching within
         the context of an entry name. If the given data type or entry does not exist in the context,
         returns an empty list.
 
         :param data_type: The data type of the records to return.
```

### Comparing `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/rules/on_save_rule_handler.py` & `sapiopycommons-32.0.0.24.5/src/sapiopycommons/rules/on_save_rule_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,14 +102,28 @@
                     data_type = "ELNSampleDetail"
                 for field_map in record_result.field_map_list:
                     rec_id: int = field_map.get("RecordId")
                     self.__field_maps.setdefault(data_type, {}).update({rec_id: field_map})
                     id_dict.setdefault(data_type, {}).update({rec_id: field_map})
             self.__base_id_to_field_maps.update({record_id: id_dict})
 
+    def get_base_record_ids(self) -> list[int]:
+        """
+        :return: A list of the record IDs that may be used with the get_records and get_models functions. These are the
+            record IDs to the records that caused the rule to trigger.
+        """
+        return list(self.__base_id_to_records.keys())
+
+    def get_field_maps_base_record_ids(self) -> list[int]:
+        """
+        :return: A list of the record IDs that may be used with the get_field_maps function. These are the
+            record IDs to the records that caused the rule to trigger.
+        """
+        return list(self.__base_id_to_field_maps.keys())
+
     def get_records(self, data_type: str, record_id: int | None = None) -> list[DataRecord]:
         """
         Get records from the cached context with the given data type. Capable of being filtered to searching within
         the context of a record ID. If the given data type or record ID does not exist in the context,
         returns an empty list.
 
         :param data_type: The data type of the records to return.
```

### Comparing `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/webhook/webhook_handlers.py` & `sapiopycommons-32.0.0.24.5/src/sapiopycommons/webhook/webhook_handlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import traceback
 from abc import abstractmethod
 from logging import Logger
 
+from sapiopylib.rest.DataMgmtService import DataMgmtServer
 from sapiopylib.rest.DataRecordManagerService import DataRecordManager
 from sapiopylib.rest.WebhookService import AbstractWebhookHandler
-from sapiopylib.rest.pojo.webhook.ClientCallbackResult import FormEntryDialogResult
 from sapiopylib.rest.pojo.webhook.WebhookContext import SapioWebhookContext
 from sapiopylib.rest.pojo.webhook.WebhookEnums import WebhookEndpointType
 from sapiopylib.rest.pojo.webhook.WebhookResult import SapioWebhookResult
 from sapiopylib.rest.utils.recordmodel.RecordModelManager import RecordModelManager, RecordModelInstanceManager, \
     RecordModelRelationshipManager
 from sapiopylib.rest.utils.recordmodel.ancestry import RecordModelAncestorManager
 
-from sapiopycommons.general.exceptions import SapioUserErrorException, SapioCriticalErrorException
-from sapiopycommons.general.popup_util import PopupUtil
+from sapiopycommons.general.exceptions import SapioUserErrorException, SapioCriticalErrorException, \
+    SapioUserCancelledException
 
 
 # FR-46064 - Initial port of PyWebhookUtils to sapiopycommons.
 class CommonsWebhookHandler(AbstractWebhookHandler):
     """
     A subclass of AbstractWebhookHandler that provides additional quality of life features, including exception
     handling for special sapiopycommons exceptions, logging, easy access invocation type methods, and the context and
@@ -40,55 +40,36 @@
 
         self.dr_man = context.data_record_manager
         self.rec_man = RecordModelManager(context.user)
         self.inst_man = self.rec_man.instance_manager
         self.rel_man = self.rec_man.relationship_manager
         self.an_man = RecordModelAncestorManager(self.rec_man)
 
-        # Handle any client callback results that may have been sent due to an exception.
-        exception_result: SapioWebhookResult | None = self.handle_exception_callback()
-        if exception_result is not None:
-            return exception_result
-
         # Wrap the execution of each webhook in a try/catch. If an exception occurs, handle any special sapiopycommons
         # exceptions. Otherwise, return a generic message stating that an error occurred.
         try:
             return self.execute(context)
         except SapioUserErrorException as e:
             return self.handle_user_error_exception(e)
         except SapioCriticalErrorException as e:
             return self.handle_critical_error_exception(e)
+        except SapioUserCancelledException as e:
+            return self.handle_user_cancelled_exception(e)
         except Exception as e:
             return self.handle_unexpected_exception(e)
 
     @abstractmethod
     def execute(self, context: SapioWebhookContext) -> SapioWebhookResult:
         """
         The business logic of the webhook, implemented in all subclasses that are called as endpoints.
         """
         pass
 
     # CR-46153: Make CommonsWebhookHandler exception handling more easily overridable by splitting them out of
     # the run method and into their own functions.
-    def handle_exception_callback(self) -> SapioWebhookResult | None:
-        """
-        Handle any client callbacks made as the result of exceptions. Whether a result is from an exception is
-        determined by reading the callback context data. Context data for exceptions should be something unique that
-        no programmer would use in practice so that we don't accidentally handle callbacks we shouldn't.
-
-        :return: A SapioWebhookResult for any handled exceptions. None if nothing was handled.
-        """
-        # Catch any SapioCriticalErrorException results.
-        result = self.context.client_callback_result
-        if result is not None:
-            result_context = result.callback_context_data
-            if isinstance(result, FormEntryDialogResult) and result_context == "SapioCriticalErrorException":
-                return SapioWebhookResult(False)
-        return None
-
     def handle_user_error_exception(self, e: SapioUserErrorException) -> SapioWebhookResult:
         """
         Handle a SapioUserErrorException. Default behavior returns the error message as display text in a webhook
         result.
 
         :param e: The exception that was raised.
         :return: A SapioWebhookResult reporting the exception to the user.
@@ -97,27 +78,25 @@
         if result is not None:
             return result
         self.log_error(traceback.format_exc())
         return SapioWebhookResult(False, display_text=e.args[0])
 
     def handle_critical_error_exception(self, e: SapioCriticalErrorException) -> SapioWebhookResult:
         """
-        Handle a SapioCriticalErrorException. Default behavior returns a FormEntryDialogRequest with an uneditable
-        text entry containing the error message. This client callback for this request is handled by
-        handle_exception_callback.
+        Handle a SapioCriticalErrorException. Default behavior makes a display_error client callback.
 
         :param e: The exception that was raised.
         :return: A SapioWebhookResult reporting the exception to the user.
         """
         result: SapioWebhookResult | None = self.handle_any_exception(e)
         if result is not None:
             return result
         self.log_error(traceback.format_exc())
-        return PopupUtil.string_field_popup("Error", "", "Reason", e.args[0],
-                                            request_context="SapioCriticalErrorException", num_lines=10)
+        DataMgmtServer.get_client_callback(self.context.user).display_error(e.args[0])
+        return SapioWebhookResult(False)
 
     def handle_unexpected_exception(self, e: Exception) -> SapioWebhookResult:
         """
         Handle a generic exception which isn't a SapioUserErrorException or SapioCriticalErrorException. Default
         behavior returns a generic error message as display text informing the user to contact Sapio support.
 
         :param e: The exception that was raised.
@@ -126,14 +105,27 @@
         result: SapioWebhookResult | None = self.handle_any_exception(e)
         if result is not None:
             return result
         self.log_error(traceback.format_exc())
         return SapioWebhookResult(False, display_text="Unexpected error occurred during webhook execution. "
                                                       "Please contact Sapio support.")
 
+    def handle_user_cancelled_exception(self, e: SapioUserCancelledException) -> SapioWebhookResult:
+        """
+        Handle a SapioUserCancelledException. Default behavior returns "User Cancelled" as display text in a webhook
+        result.
+
+        :param e: The exception that was raised.
+        :return: A SapioWebhookResult with display text saying the user cancelled the request.
+        """
+        result: SapioWebhookResult | None = self.handle_any_exception(e)
+        if result is not None:
+            return result
+        return SapioWebhookResult(False, display_text="User cancelled.")
+
     # noinspection PyMethodMayBeStatic,PyUnusedLocal
     def handle_any_exception(self, e: Exception) -> SapioWebhookResult | None:
         """
         An exception handler which runs regardless of the type of exception that was raised. Can be used to "rollback"
         the client if an error occurs. Default behavior does nothing and returns None.
 
         :param e: The exception that was raised.
```

### Comparing `sapiopycommons-31.3.0.23.12.3/LICENSE` & `sapiopycommons-32.0.0.24.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sapiopycommons-31.3.0.23.12.3/README.md` & `sapiopycommons-32.0.0.24.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 pypi.org is granted the right to distribute sapiopycommons forever.
 
 This license does not provide any rights to use any other copyrighted artifacts from Sapio Sciences. (And they are typically written in another programming language with no linkages to this library.)
 
 ## Dependencies
 The following dependencies are required for this package:
 - [sapiopylib - The official Sapio Informatics Platform Python API package.](https://pypi.org/project/sapiopylib/)
+- [databind - Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses.](https://pypi.org/project/databind/)
 
 ## Getting Help
 If you have a support contract with Sapio Sciences, please use our [technical support channels](https://sapio-sciences.atlassian.net/servicedesk/customer/portals).
 
 ## About Us
 Sapio is at the forefront of the Digital Lab with its science-aware platform for managing all your life science data with its integrated Electronic Lab Notebook, LIMS Software and Scientific Data Management System.
```

#### html2text {}

```diff
@@ -12,14 +12,16 @@
 library version to ensure it is compatible with your Sapio Informatics
 Platform. ## Licenses sapiopycommons is licensed under MPL 2.0. pypi.org is
 granted the right to distribute sapiopycommons forever. This license does not
 provide any rights to use any other copyrighted artifacts from Sapio Sciences.
 (And they are typically written in another programming language with no
 linkages to this library.) ## Dependencies The following dependencies are
 required for this package: - [sapiopylib - The official Sapio Informatics
-Platform Python API package.](https://pypi.org/project/sapiopylib/) ## Getting
-Help If you have a support contract with Sapio Sciences, please use our
-[technical support channels](https://sapio-sciences.atlassian.net/servicedesk/
-customer/portals). ## About Us Sapio is at the forefront of the Digital Lab
-with its science-aware platform for managing all your life science data with
-its integrated Electronic Lab Notebook, LIMS Software and Scientific Data
-Management System. Visit us at _S_a_p_i_o_ _S_c_i_e_n_c_e_s.
+Platform Python API package.](https://pypi.org/project/sapiopylib/) - [databind
+- Databind is a library inspired by jackson-databind to de-/serialize Python
+dataclasses.](https://pypi.org/project/databind/) ## Getting Help If you have a
+support contract with Sapio Sciences, please use our [technical support
+channels](https://sapio-sciences.atlassian.net/servicedesk/customer/portals).
+## About Us Sapio is at the forefront of the Digital Lab with its science-aware
+platform for managing all your life science data with its integrated Electronic
+Lab Notebook, LIMS Software and Scientific Data Management System. Visit us at
+_S_a_p_i_o_ _S_c_i_e_n_c_e_s.
```

### Comparing `sapiopycommons-31.3.0.23.12.3/pyproject.toml` & `sapiopycommons-32.0.0.24.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sapiopycommons"
-version='31.3.0.23.12.3'
+version='32.0.0.24.5'
 authors = [
     { name="Jonathan Steck", email="jsteck@sapiosciences.com" },
     { name="Yechen Qiao", email="yqiao@sapiosciences.com" },
 ]
 description = "Official Sapio Python API Utilities Package"
 license = "MPL-2.0"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
-        'sapiopylib>=2023.12.13.174'
+        'sapiopylib>=2024.4.23a188', 'databind>=4.5'
 ]
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Healthcare Industry",
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
```

### Comparing `sapiopycommons-31.3.0.23.12.3/PKG-INFO` & `sapiopycommons-32.0.0.24.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sapiopycommons
-Version: 31.3.0.23.12.3
+Version: 32.0.0.24.5
 Summary: Official Sapio Python API Utilities Package
 Project-URL: Homepage, https://github.com/sapiosciences
 Author-email: Jonathan Steck <jsteck@sapiosciences.com>, Yechen Qiao <yqiao@sapiosciences.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
 Keywords: eln,lims,rest,sapio
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
-Requires-Dist: sapiopylib>=2023.12.13.174
+Requires-Dist: databind>=4.5
+Requires-Dist: sapiopylib>=2024.4.23a188
 Description-Content-Type: text/markdown
 
 
 # sapiopycommons: Official Sapio Python API Utilities Package
 
 <div align="center"><a href="https://www.sapiosciences.com" target="_blank">
   <img src="https://s3.amazonaws.com/public.exemplareln.com/sapio-pylib/sapio-sciencesofficial-python-api-library.png" alt="Sapio Sciences"><br>
@@ -46,14 +47,15 @@
 pypi.org is granted the right to distribute sapiopycommons forever.
 
 This license does not provide any rights to use any other copyrighted artifacts from Sapio Sciences. (And they are typically written in another programming language with no linkages to this library.)
 
 ## Dependencies
 The following dependencies are required for this package:
 - [sapiopylib - The official Sapio Informatics Platform Python API package.](https://pypi.org/project/sapiopylib/)
+- [databind - Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses.](https://pypi.org/project/databind/)
 
 ## Getting Help
 If you have a support contract with Sapio Sciences, please use our [technical support channels](https://sapio-sciences.atlassian.net/servicedesk/customer/portals).
 
 ## About Us
 Sapio is at the forefront of the Digital Lab with its science-aware platform for managing all your life science data with its integrated Electronic Lab Notebook, LIMS Software and Scientific Data Management System.
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.3 Name: sapiopycommons Version: 31.3.0.23.12.3 Summary:
+Metadata-Version: 2.3 Name: sapiopycommons Version: 32.0.0.24.5 Summary:
 Official Sapio Python API Utilities Package Project-URL: Homepage, https://
 github.com/sapiosciences Author-email: Jonathan Steck
 sapiosciences.com>, Yechen Qiao
 sapiosciences.com> License-Expression: MPL-2.0 License-File: LICENSE Keywords:
 eln,lims,rest,sapio Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Healthcare Industry Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3.10 Classifier: Topic :: Scientific/Engineering :: Bio-
 Informatics Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Requires-Python: >=3.10 Requires-Dist: sapiopylib>=2023.12.13.174
-Description-Content-Type: text/markdown # sapiopycommons: Official Sapio Python
-API Utilities Package
+Modules Requires-Python: >=3.10 Requires-Dist: databind>=4.5 Requires-Dist:
+sapiopylib>=2024.4.23a188 Description-Content-Type: text/markdown #
+sapiopycommons: Official Sapio Python API Utilities Package
                                _[_S_a_p_i_o_ _S_c_i_e_n_c_e_s_]
 ----------------- [![PyPI Latest Release](https://img.shields.io/pypi/v/
 sapiopycommons.svg)](https://pypi.org/project/sapiopycommons/) [![License]
 (https://img.shields.io/pypi/l/sapiopycommons.svg)](https://github.com/
 sapiosciences/sapio-py-tutorials/blob/master/LICENSE) ## What is it?
 sapiopycommons is a utilities package, developed and maintained by Sapio
 Sciences, designed to be used in conjunction with sapiopylib. It provides
@@ -26,14 +26,16 @@
 library version to ensure it is compatible with your Sapio Informatics
 Platform. ## Licenses sapiopycommons is licensed under MPL 2.0. pypi.org is
 granted the right to distribute sapiopycommons forever. This license does not
 provide any rights to use any other copyrighted artifacts from Sapio Sciences.
 (And they are typically written in another programming language with no
 linkages to this library.) ## Dependencies The following dependencies are
 required for this package: - [sapiopylib - The official Sapio Informatics
-Platform Python API package.](https://pypi.org/project/sapiopylib/) ## Getting
-Help If you have a support contract with Sapio Sciences, please use our
-[technical support channels](https://sapio-sciences.atlassian.net/servicedesk/
-customer/portals). ## About Us Sapio is at the forefront of the Digital Lab
-with its science-aware platform for managing all your life science data with
-its integrated Electronic Lab Notebook, LIMS Software and Scientific Data
-Management System. Visit us at _S_a_p_i_o_ _S_c_i_e_n_c_e_s.
+Platform Python API package.](https://pypi.org/project/sapiopylib/) - [databind
+- Databind is a library inspired by jackson-databind to de-/serialize Python
+dataclasses.](https://pypi.org/project/databind/) ## Getting Help If you have a
+support contract with Sapio Sciences, please use our [technical support
+channels](https://sapio-sciences.atlassian.net/servicedesk/customer/portals).
+## About Us Sapio is at the forefront of the Digital Lab with its science-aware
+platform for managing all your life science data with its integrated Electronic
+Lab Notebook, LIMS Software and Scientific Data Management System. Visit us at
+_S_a_p_i_o_ _S_c_i_e_n_c_e_s.
```

