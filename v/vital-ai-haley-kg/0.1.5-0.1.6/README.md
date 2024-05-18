# Comparing `tmp/vital-ai-haley-kg-0.1.5.tar.gz` & `tmp/vital-ai-haley-kg-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vital-ai-haley-kg-0.1.5.tar", last modified: Fri May 17 18:02:01 2024, max compression
+gzip compressed data, was "vital-ai-haley-kg-0.1.6.tar", last modified: Sat May 18 22:40:37 2024, max compression
```

## Comparing `vital-ai-haley-kg-0.1.5.tar` & `vital-ai-haley-kg-0.1.6.tar`

### file list

```diff
@@ -1,912 +1,922 @@
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-17 18:02:01.584804 vital-ai-haley-kg-0.1.5/
--rw-r--r--   0 hadfield   (501) staff       (20)      501 2024-05-17 18:02:01.584548 vital-ai-haley-kg-0.1.5/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 17:06:26.000000 vital-ai-haley-kg-0.1.5/README.md
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-17 18:02:01.404421 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:39:48.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-17 18:02:01.532594 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/
--rw-r--r--   0 hadfield   (501) staff       (20)     1403 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/DomainCategory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/DomainCategory.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)      178 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/DomainOntology.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasActorKGFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasActorKGFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasAgentKGFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasAgentKGFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1313 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasChatMessageKGFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasChatMessageKGFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasDocumentKGFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasDocumentKGFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasEntityKGFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasEntityKGFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasEntityKGStatement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasEntityKGStatement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1340 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasEntityTypePartOfKGFrameType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasEntityTypePartOfKGFrameType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasEventKGFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasEventKGFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasGroupKGFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasGroupKGFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1325 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasIncomingKGRelationType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasIncomingKGRelationType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1322 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasInteractionKGDocument.py
--rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasInteractionKGDocument.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasInteractionKGEntity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasInteractionKGEntity.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1313 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasInteractionKGFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasInteractionKGFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1289 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGActor.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGActor.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGAgent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGAgent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1313 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGAgentDuplicate.py
--rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGAgentDuplicate.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1307 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGAgentPublisher.py
--rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGAgentPublisher.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGAggregation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGAggregation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGAnnotation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGAnnotation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGBroadCategory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGBroadCategory.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1527 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGCategory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGCategory.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGChatMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGChatMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGCriterion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGCriterion.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1289 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGDocument.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGDocument.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1313 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGDocumentFileNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGDocumentFileNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGDocumentSegment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGDocumentSegment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2346 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGEdge.py
--rw-r--r--   0 hadfield   (501) staff       (20)      426 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGEdge.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1283 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGEntity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGEntity.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGEntityMention.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGEntityMention.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGExtractTask.py
--rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGExtractTask.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1834 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGExtraction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      279 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGExtraction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1283 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGFigure.py
--rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGFigure.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1283 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGFlag.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGFlag.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1382 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGGroup.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGGroup.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1331 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGIndexDocumentAttempt.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGIndexDocumentAttempt.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1334 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGIndexDocumentCategory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGIndexDocumentCategory.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1334 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGIndexDocumentFileNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGIndexDocumentFileNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGInstruction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGInstruction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1328 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGInteractionDependency.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGInteractionDependency.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1319 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGInteractionElement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGInteractionElement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGMedia.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGMedia.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGMediaFileNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGMediaFileNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1307 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGNarrowCategory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGNarrowCategory.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1283 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1313 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGNormalizedEntity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGNormalizedEntity.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGOrganization.py
--rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGOrganization.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1283 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGPath.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGPath.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGPathElement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGPathElement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGPointer.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGPointer.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1325 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGQueryCriteriaGroup.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGQueryCriteriaGroup.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1334 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGQueryExploreTraversal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGQueryExploreTraversal.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGQueryGroup.py
--rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGQueryGroup.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGQuerySort.py
--rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGQuerySort.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1313 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGQueryTraversal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGQueryTraversal.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1283 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRating.py
--rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRating.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRatingSummary.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRatingSummary.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRefEdge.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRefEdge.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1527 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRefRelation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRefRelation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1509 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRelation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      196 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRelation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1635 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRelationMention.py
--rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRelationMention.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1289 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGResource.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGResource.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRunDocument.py
--rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRunDocument.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1283 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGSearch.py
--rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGSearch.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1710 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1635 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGSlotProtoType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGSlotProtoType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1406 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGSlotType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      169 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGSlotType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGStatement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGStatement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGStatsSummary.py
--rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGStatsSummary.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGTable.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGTable.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGTag.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGTag.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1283 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGThread.py
--rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGThread.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGTypePath.py
--rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGTypePath.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasOrganizationKGFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasOrganizationKGFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1325 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasOutgoingKGRelationType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasOutgoingKGRelationType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1428 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasPartOfKGFrameType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasPartOfKGFrameType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1325 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasRecipientEntityKGEmail.py
--rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasRecipientEntityKGEmail.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasRequestKGFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasRequestKGFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasResourceKGFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasResourceKGFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasResponseKGFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasResponseKGFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1289 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasRunKGFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasRunKGFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSameAsKGEntity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSameAsKGEntity.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1322 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSameAsKGEntityMention.py
--rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSameAsKGEntityMention.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSameAsKGType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSameAsKGType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1322 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSearchKGEntityMention.py
--rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSearchKGEntityMention.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSenderEntityKGEmail.py
--rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSenderEntityKGEmail.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1419 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSubKGFrameType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      174 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSubKGFrameType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1286 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSubKGType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSubKGType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasTableKGFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasTableKGFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasTaskKGFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasTaskKGFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasThreadKGFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasThreadKGFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasToolResultKGFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasToolResultKGFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1326 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/HyperEdge_hasKGExtractionEdge.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/HyperEdge_hasKGExtractionEdge.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1572 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGActionStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGActionStatus.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGActionType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGActionType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1332 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGActor.py
--rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGActor.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1244 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGActorType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      106 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGActorType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     3340 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      746 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentPublishStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentPublishStatus.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1486 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentPublisher.py
--rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentPublisher.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentPublisherType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      115 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentPublisherType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentService.py
--rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentService.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2666 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentSubmission.py
--rw-r--r--   0 hadfield   (501) staff       (20)      581 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentSubmission.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1274 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentSubmissionType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      116 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentSubmissionType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1244 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      106 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1481 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAggregation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      178 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAggregation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1733 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAggregationResult.py
--rw-r--r--   0 hadfield   (501) staff       (20)      263 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAggregationResult.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAggregationType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAggregationType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1458 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAnnotation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAnnotation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1259 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAnnotationType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      111 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAnnotationType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1676 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAppEvent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAppEvent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAppEventSource.py
--rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAppEventSource.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAppEventType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAppEventType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1340 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAudio.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAudio.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1347 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAudioSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAudioSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGBeliefModeType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGBeliefModeType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1359 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGBooleanSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGBooleanSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1251 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGBracket.py
--rw-r--r--   0 hadfield   (501) staff       (20)      117 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGBracket.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1364 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCalendarEvent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCalendarEvent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1268 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCalendarEventType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      114 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCalendarEventType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1450 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCategory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCategory.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1253 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCategoryType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      109 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCategoryType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChatBotMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChatBotMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1613 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChatInteraction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChatInteraction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1274 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChatInteractionType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      116 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChatInteractionType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1908 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChatMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      304 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChatMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1262 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChatMessageType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      112 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChatMessageType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1283 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChatUserMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChatUserMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1379 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChoiceOptionSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChoiceOptionSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1354 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChoiceSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChoiceSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1799 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCodeDocument.py
--rw-r--r--   0 hadfield   (501) staff       (20)      263 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCodeDocument.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1265 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCodeDocumentType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      113 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCodeDocumentType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCodeLanguage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCodeLanguage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1343 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCodeSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCodeSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGConstraintComparator.py
--rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGConstraintComparator.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     4797 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCriterion.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1208 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCriterion.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCriterionType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCriterionType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1362 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCurrencySlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCurrencySlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1364 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDateTimeSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDateTimeSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1481 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDescriptor.py
--rw-r--r--   0 hadfield   (501) staff       (20)      180 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDescriptor.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     3603 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDocument.py
--rw-r--r--   0 hadfield   (501) staff       (20)      837 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDocument.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDocumentSegmentMethod.py
--rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDocumentSegmentMethod.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDocumentSegmentType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDocumentSegmentType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1253 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDocumentType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      109 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDocumentType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1354 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDoubleSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDoubleSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2442 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEMail.py
--rw-r--r--   0 hadfield   (501) staff       (20)      452 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEMail.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1244 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEMailType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      106 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEMailType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1238 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGElement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      104 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGElement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1970 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEntity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      303 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEntity.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1892 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEntityMention.py
--rw-r--r--   0 hadfield   (501) staff       (20)      286 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEntityMention.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1351 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEntitySlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEntitySlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1247 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEntityType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      107 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEntityType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1332 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEvent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEvent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1244 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEventType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      106 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEventType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGExpressionType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGExpressionType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1353 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGExtractTask.py
--rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGExtractTask.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGExtractor.py
--rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGExtractor.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1449 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFigure.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFigure.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1340 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFileType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFileType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1367 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFileUploadSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFileUploadSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1753 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFlag.py
--rw-r--r--   0 hadfield   (501) staff       (20)      239 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFlag.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFlagReason.py
--rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFlagReason.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFlagSource.py
--rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFlagSource.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1241 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFlagType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      105 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFlagType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1253 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFormType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      118 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFormType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2274 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      380 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1477 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFrameProtoType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      169 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFrameProtoType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1362 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFrameType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFrameType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1392 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFrameTypeDescriptor.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFrameTypeDescriptor.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1379 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGGeoLocationSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGGeoLocationSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1332 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGGroup.py
--rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGGroup.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1244 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGGroupType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      106 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGGroupType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1454 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIPAddress.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIPAddress.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1446 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGImage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGImage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1347 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGImageSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGImageSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2956 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexDocument.py
--rw-r--r--   0 hadfield   (501) staff       (20)      647 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexDocument.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1985 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexDocumentAttempt.py
--rw-r--r--   0 hadfield   (501) staff       (20)      354 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexDocumentAttempt.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1320 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexDocumentAttemptStatusType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexDocumentAttemptStatusType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1311 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexDocumentClassification.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexDocumentClassification.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexDocumentStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexDocumentStatus.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1302 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexDocumentStorageType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexDocumentStorageType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexStatus.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1465 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGInstruction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGInstruction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1262 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGInstructionType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      112 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGInstructionType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1359 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIntegerSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIntegerSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1468 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGInteraction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGInteraction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1262 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGInteractionType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      112 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGInteractionType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1346 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGJSONSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGJSONSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1344 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGLongSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGLongSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1362 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGLongTextSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGLongTextSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1553 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGMedia.py
--rw-r--r--   0 hadfield   (501) staff       (20)      181 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGMedia.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1254 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGMetaType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      118 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGMetaType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1393 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGMultiChoiceOptionSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGMultiChoiceOptionSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1375 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGMultiChoiceSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGMultiChoiceSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGMultiTaxonomyOptionSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGMultiTaxonomyOptionSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1380 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGMultiTaxonomySlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGMultiTaxonomySlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1484 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGNewsEntity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      182 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGNewsEntity.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2544 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      493 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1364 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGNodeProxy.py
--rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGNodeProxy.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1584 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGNoteDocument.py
--rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGNoteDocument.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1265 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGNoteDocumentType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      113 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGNoteDocumentType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1360 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGOrganization.py
--rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGOrganization.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1265 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGOrganizationType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      113 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGOrganizationType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1242 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGPath.py
--rw-r--r--   0 hadfield   (501) staff       (20)      114 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGPath.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGPathElement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGPathElement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1547 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGPlace.py
--rw-r--r--   0 hadfield   (501) staff       (20)      178 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGPlace.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1563 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGPointer.py
--rw-r--r--   0 hadfield   (501) staff       (20)      196 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGPointer.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1262 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGProductEntity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      116 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGProductEntity.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1828 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGPropertySlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      295 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGPropertySlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGProvenanceType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGProvenanceType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1354 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQuery.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQuery.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1274 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryANDGroup.py
--rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryANDGroup.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1322 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryCriteriaANDGroup.py
--rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryCriteriaANDGroup.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryCriteriaGroup.py
--rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryCriteriaGroup.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1319 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryCriteriaORGroup.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryCriteriaORGroup.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryExploreTraversal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryExploreTraversal.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryGroup.py
--rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryGroup.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryORGroup.py
--rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryORGroup.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1476 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQuerySort.py
--rw-r--r--   0 hadfield   (501) staff       (20)      180 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQuerySort.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQuerySortDirection.py
--rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQuerySortDirection.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQuerySortType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQuerySortType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryTraversal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryTraversal.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2098 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRating.py
--rw-r--r--   0 hadfield   (501) staff       (20)      350 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRating.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRatingSource.py
--rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRatingSource.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2654 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRatingSummary.py
--rw-r--r--   0 hadfield   (501) staff       (20)      584 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRatingSummary.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1268 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRatingSummaryType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      114 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRatingSummaryType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1247 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRatingType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      107 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRatingType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRatingValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRatingValue.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRatingValueType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRatingValueType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1368 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRelationType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRelationType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2150 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRelationTypeRestriction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      443 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRelationTypeRestriction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1349 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRequest.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRequest.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1250 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRequestType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      108 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRequestType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1563 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGResource.py
--rw-r--r--   0 hadfield   (501) staff       (20)      188 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGResource.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1253 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGResourceType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      109 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGResourceType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1454 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGResponse.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1253 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGResponseType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      109 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGResponseType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1463 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRunDocument.py
--rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRunDocument.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1262 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRunDocumentType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      112 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRunDocumentType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1339 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRunSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRunSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1446 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSearch.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSearch.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1247 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSearchType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      107 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSearchType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2178 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      360 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotConstraintType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotConstraintType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1472 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotProtoType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotProtoType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1252 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotRoleType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      109 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotRoleType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1385 2024-05-04 22:21:49.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotTypDescriptor.py
--rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 22:21:49.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotTypDescriptor.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1678 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1387 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotTypeDescriptor.py
--rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotTypeDescriptor.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotValueType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotValueType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1349 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGStatement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGStatement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2055 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGStatsSummary.py
--rw-r--r--   0 hadfield   (501) staff       (20)      364 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGStatsSummary.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1265 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGStatsSummaryType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      113 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGStatsSummaryType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1232 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTable.py
--rw-r--r--   0 hadfield   (501) staff       (20)      102 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTable.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1425 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTag.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTag.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1238 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTagType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      104 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTagType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1328 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTask.py
--rw-r--r--   0 hadfield   (501) staff       (20)      117 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTask.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1241 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTaskType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      105 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTaskType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1379 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTaxonomyOptionSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTaxonomyOptionSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1359 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTaxonomySlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTaxonomySlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1680 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTenant.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTenant.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1346 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTextSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTextSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1235 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGThread.py
--rw-r--r--   0 hadfield   (501) staff       (20)      103 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGThread.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1352 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGToolResult.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGToolResult.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1259 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGToolResultType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      111 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGToolResultType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1562 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      192 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1259 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTypeMethod.py
--rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTypeMethod.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     3229 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTypePath.py
--rw-r--r--   0 hadfield   (501) staff       (20)      656 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTypePath.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTypeRestriction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTypeRestriction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1339 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGURISlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGURISlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     3082 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGUserContext.py
--rw-r--r--   0 hadfield   (501) staff       (20)      700 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGUserContext.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGValidType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGValidType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1340 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGVideo.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGVideo.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1347 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGVideoSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGVideoSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1245 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGVisit.py
--rw-r--r--   0 hadfield   (501) staff       (20)      115 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGVisit.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1486 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGWebEntity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      183 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGWebEntity.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/NewsCategory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/NewsCategory.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/NewsContentCategory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-17 17:59:24.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/NewsContentCategory.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:39:48.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-17 18:02:01.583026 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasAnnotationText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasAudioSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasBooleanSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasChoiceSlotOptionValues.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasChoiceSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasCodeSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasCurrencySlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasDateTimeSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      262 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasDestinationRelationTypeRestrictionURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasDocumentAttemptDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasDocumentAttemptStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasDocumentAttemptStatusCode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasDocumentAuthorList.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasDocumentContentPath.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasDocumentContentType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasDocumentCorrectedURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasDocumentDescription.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasDocumentHTMLContent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasDocumentHeadline.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasDocumentOriginalURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasDocumentPublicationDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasDocumentRetrievalDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasDocumentURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasDocumentVersion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasDomainCategoryIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasDoubleSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasEdgeName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasEntitySlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasFileUploadSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasFrameGraphURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasFrameSequence.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasGeoLocationSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasHaleyRegionURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasImageSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasIntegerSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasInteractionSequence.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasJsonSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGActionAttemptDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGActionStatusURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGActionType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGActionTypeList.py
--rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGActionTypeSummaryDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGActorType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentAvatarImageSourceURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentAvatarImageURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentAvatarLargeImageURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentDeploymentURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentDescription.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentImplIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentModificationDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentNameSlug.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentPublishStatusURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentPublisherName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentPublisherType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentPublisherWebsiteURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentRankingScore.py
--rw-r--r--   0 hadfield   (501) staff       (20)      254 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentRankingScoreUpdateDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentServiceURIs.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentSubmissionComments.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentSubmissionCreator.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentSubmissionDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentSubmissionDescription.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentSubmissionName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      250 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentSubmissionSubmitterEmail.py
--rw-r--r--   0 hadfield   (501) staff       (20)      248 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentSubmissionSubmitterName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentSubmissionType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentSubmissionURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAgentType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAggregationDoubleValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAggregationIntegerValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAggregationName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAggregationTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAnnotationType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAppEventActorURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAppEventAgent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAppEventSourceURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGAppEventType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGBeliefModeType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGBracketURIs.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGCalendarEventType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGCategoryType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGChatInteractionCompleteText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGChatInteractionSummaryText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGChatInteractionType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGChatInteractionURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGChatMessageDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGChatMessageSequence.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGChatMessageText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGChatMessageType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGCodeDocumentType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGCodeInterpreterVersion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGCodeLanguageURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGCodeLanguageVersion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGConstraintComparatorURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGContentType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGCriterionTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGDataHash.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGDescriptorLabel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGDescriptorLanguageURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGDocumentContent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGDocumentDescription.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGDocumentEndTokenIndex.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGDocumentExtractedContent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGDocumentHTMLContent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGDocumentHeadline.py
--rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGDocumentPublicationDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGDocumentRetrievalDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGDocumentSegmentIndex.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGDocumentSegmentMethodURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGDocumentSegmentTokenLength.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGDocumentSegmentTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGDocumentStartTokenIndex.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGDocumentSummary.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGDocumentTokenLength.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGDocumentType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGDocumentURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGEMailType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGEmailBCCAddressList.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGEmailCCAddressList.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGEmailRecipientAddress.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGEmailRecipientName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGEmailSendDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGEmailSenderAddress.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGEmailSenderName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGEmailSubject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGEmailSummary.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGEmailToAddressList.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGEncodedByteData.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGEndByteIndex.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGEndTokenIndex.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGEntityAccountURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGEntityLoginURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGEntityType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGEntityTypeDescription.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGEventType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGExpressionType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGExtractTaskURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGExtractorURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGFileType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGFlagDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGFlagDescription.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGFlagReasonURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGFlagSourceURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGFlagType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGFormType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGFrameType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGFrameTypeDescription.py
--rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGFrameTypeExternIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGGraphAssertionDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGGroupType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGIPAddress.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGIPAddressJSON.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGIndexDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      258 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGIndexDocumentAttemptStatusTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGIndexDocumentClassificationURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGIndexDocumentStatusURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGIndexDocumentStorageTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGIndexStatusURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGInstructionText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGInstructionType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGInteractionType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGMediaDuration.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGMediaEncoding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGModelVersion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGNewsEntityBiasMetric.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGNewsEntityPrimaryDomain.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGNodeCacheDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGNodeReferenceURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGNoteDocumentContent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGNoteDocumentTitle.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGNoteDocumentType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGOrganizationType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGPixelHeight.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGPixelWidth.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGPlaceIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGPlaceJSON.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGPlaceURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGPointerNextURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGPointerPriorURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGPointerURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGPropertyGroupNameSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGPropertyNameSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGProvenanceType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryBooleanValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryChoiceValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryDateTimeValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryDoubleValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryIntegerValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryKGMetaType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryKGNodeClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryKGRelationType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryKGType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryLongTextValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryMoveFromConcepts.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryMoveToConcepts.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryMultiChoiceValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryMultiTaxonomyValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryNearVectorCertainty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryNearVectorDistance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryNearVectorForce.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryObjectURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryPropertyURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryProvenanceURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryRootURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQuerySerializedVector.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQuerySortDirectionURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQuerySortTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryTaxonomyValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryTextValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryTopKLimit.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryURIValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGQueryUnknownValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRatingCalculationDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRatingDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRatingDescription.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRatingSourceURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRatingStarValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      256 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRatingSummaryAverageRatingDouble.py
--rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRatingSummaryAverageStarRating.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRatingSummaryNegativeCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRatingSummaryNeutralCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRatingSummaryPositiveCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRatingSummaryReviewCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRatingSummaryText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRatingSummaryTitle.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRatingSummaryTotalCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRatingSummaryType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRatingType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRatingValueDouble.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRatingValueTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRatingValueURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRelationType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRelationTypeDescription.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRelationTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRequestType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRequestURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGResourceDescription.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGResourceName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGResourceType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGResponseType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRunCodeOutput.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGRunDocumentType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGSearchDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGSearchType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGSlotConstraintType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGSlotReferenceURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGSlotRoleSequence.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGSlotRoleType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGSlotType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGSlotTypeClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGSlotTypeDescription.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGSlotTypeExternIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGSlotTypeLabel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGSlotTypeName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGSlotValueType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGSourceCode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGStartByteIndex.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGStartTokenIndex.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGStatsSummaryCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGStatsSummaryCountPercentage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGStatsSummaryPeriod.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGStatsSummaryPeriodDay.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGStatsSummaryPeriodMonth.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGStatsSummaryPeriodYear.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGStatsSummaryType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGTagName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGTagType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGTaskType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGTaxonomyOptionURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGTenantAccountID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGTenantAccountURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGTenantIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGToolResultType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGTypeClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGTypeMethodURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGTypeVersion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGUserContextAccountLevel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGUserContextAccountURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGUserContextAgentFamiliarity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGUserContextAgentTone.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGUserContextCurrentDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGUserContextCurrentTimezone.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGUserContextExperienceLevel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGUserContextGender.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGUserContextLightLevel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGUserContextLocation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGUserContextLoginURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGUserContextMood.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGUserContextName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGUserContextPronoun.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGUserContextSoundLevel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGValidTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGVersion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGWebEntityDomainCategories.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGWebEntityPrimaryDomain.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasKGraphDescription.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasLongSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasLongTextSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasMultiChoiceSlotValues.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasMultiTaxonomySlotValues.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasParentFrameURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasPrimaryLanguageType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasPropertyClassSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasPropertyFrameTypeSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasPropertySlotTypeSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasRunSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasSlotSequence.py
--rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasSourceRelationTypeRestrictionURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasStatementText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasTaxonomySlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasTextSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasTopCategoryURIs.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasUriSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_hasVideoSlotValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_isKGAgentSubmissionApproved.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_isKGAgentSubmissionConverted.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_isKGAgentSubmissionReviewed.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_isKGCategoryRoot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_isKGGlobalTenant.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_isKGQuerySubclassExpansion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_isKGQuerySubtypeExpansion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_isKGRelationTypeDestinationOpen.py
--rw-r--r--   0 hadfield   (501) staff       (20)      248 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_isKGRelationTypeExpandDestination.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_isKGRelationTypeExpandSource.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_isKGRelationTypeSourceOpen.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-17 17:59:25.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/Property_isKGRelationTypeSymmetric.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:39:48.000000 vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/properties/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-17 18:02:01.584856 vital-ai-haley-kg-0.1.5/setup.cfg
--rw-r--r--   0 hadfield   (501) staff       (20)      896 2024-05-17 18:00:42.000000 vital-ai-haley-kg-0.1.5/setup.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-17 18:02:01.584183 vital-ai-haley-kg-0.1.5/vital_ai_haley_kg.egg-info/
--rw-r--r--   0 hadfield   (501) staff       (20)      501 2024-05-17 18:02:01.000000 vital-ai-haley-kg-0.1.5/vital_ai_haley_kg.egg-info/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)    49699 2024-05-17 18:02:01.000000 vital-ai-haley-kg-0.1.5/vital_ai_haley_kg.egg-info/SOURCES.txt
--rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-17 18:02:01.000000 vital-ai-haley-kg-0.1.5/vital_ai_haley_kg.egg-info/dependency_links.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       62 2024-05-17 18:02:01.000000 vital-ai-haley-kg-0.1.5/vital_ai_haley_kg.egg-info/entry_points.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       31 2024-05-17 18:02:01.000000 vital-ai-haley-kg-0.1.5/vital_ai_haley_kg.egg-info/requires.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       19 2024-05-17 18:02:01.000000 vital-ai-haley-kg-0.1.5/vital_ai_haley_kg.egg-info/top_level.txt
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-18 22:40:37.675841 vital-ai-haley-kg-0.1.6/
+-rw-r--r--   0 hadfield   (501) staff       (20)      501 2024-05-18 22:40:37.675458 vital-ai-haley-kg-0.1.6/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 17:06:26.000000 vital-ai-haley-kg-0.1.6/README.md
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-18 22:40:37.502015 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:39:48.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-18 22:40:37.608326 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/
+-rw-r--r--   0 hadfield   (501) staff       (20)     1403 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/DomainCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/DomainCategory.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)      178 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/DomainOntology.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasActorKGFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasActorKGFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasAgentKGFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasAgentKGFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1313 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasChatMessageKGFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasChatMessageKGFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasDocumentKGFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasDocumentKGFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasEntityKGFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasEntityKGFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasEntityKGStatement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasEntityKGStatement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1340 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasEntityTypePartOfKGFrameType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasEntityTypePartOfKGFrameType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasEventKGFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasEventKGFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasGroupKGFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasGroupKGFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1325 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasIncomingKGRelationType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasIncomingKGRelationType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1322 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasInteractionKGDocument.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasInteractionKGDocument.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasInteractionKGEntity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasInteractionKGEntity.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1313 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasInteractionKGFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasInteractionKGFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1289 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGActor.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGActor.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGAgent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGAgent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1313 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGAgentDuplicate.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGAgentDuplicate.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1307 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGAgentPublisher.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGAgentPublisher.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGAggregation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGAggregation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGAnnotation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGAnnotation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGBroadCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGBroadCategory.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1527 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGCategory.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1309 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGChatInteraction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGChatInteraction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGChatMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGChatMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGCriterion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGCriterion.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1289 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGDocument.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGDocument.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1313 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGDocumentFileNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGDocumentFileNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGDocumentSegment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGDocumentSegment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2346 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGEdge.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      426 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGEdge.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1283 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGEntity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGEntity.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGEntityMention.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGEntityMention.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGExtractTask.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGExtractTask.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1834 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGExtraction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      279 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGExtraction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1283 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGFigure.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGFigure.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1283 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGFlag.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGFlag.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1382 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGGroup.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGGroup.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1331 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGIndexDocumentAttempt.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGIndexDocumentAttempt.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1334 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGIndexDocumentCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGIndexDocumentCategory.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1334 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGIndexDocumentFileNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGIndexDocumentFileNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGInstruction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGInstruction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1328 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGInteractionDependency.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGInteractionDependency.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1319 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGInteractionElement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGInteractionElement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGMedia.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGMedia.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGMediaFileNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGMediaFileNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1307 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGNarrowCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGNarrowCategory.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1283 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1313 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGNormalizedEntity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGNormalizedEntity.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGOrganization.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGOrganization.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1283 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGPath.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGPath.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGPathElement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGPathElement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGPointer.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGPointer.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1325 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGQueryCriteriaGroup.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGQueryCriteriaGroup.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1334 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGQueryExploreTraversal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGQueryExploreTraversal.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGQueryGroup.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGQueryGroup.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGQuerySort.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGQuerySort.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1313 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGQueryTraversal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGQueryTraversal.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1283 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRating.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRating.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRatingSummary.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRatingSummary.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRefEdge.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRefEdge.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1527 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRefRelation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRefRelation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1509 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRelation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      196 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRelation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1635 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRelationMention.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRelationMention.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1289 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGResource.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGResource.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRunDocument.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRunDocument.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1283 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGSearch.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGSearch.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1710 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1635 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGSlotProtoType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGSlotProtoType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1406 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGSlotType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      169 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGSlotType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGStatement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGStatement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGStatsSummary.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGStatsSummary.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGTable.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGTable.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGTag.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGTag.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1283 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGThread.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGThread.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGTypePath.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGTypePath.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasOrganizationKGFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasOrganizationKGFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1325 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasOutgoingKGRelationType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasOutgoingKGRelationType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1428 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasPartOfKGFrameType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasPartOfKGFrameType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1325 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasRecipientEntityKGEmail.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasRecipientEntityKGEmail.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasRequestKGFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasRequestKGFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasResourceKGFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasResourceKGFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasResponseKGFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasResponseKGFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1289 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasRunKGFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasRunKGFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSameAsKGEntity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSameAsKGEntity.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1322 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSameAsKGEntityMention.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSameAsKGEntityMention.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSameAsKGType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSameAsKGType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1322 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSearchKGEntityMention.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSearchKGEntityMention.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSenderEntityKGEmail.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSenderEntityKGEmail.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1419 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSubKGFrameType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      174 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSubKGFrameType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1286 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSubKGType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSubKGType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasTableKGFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasTableKGFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasTaskKGFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasTaskKGFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasThreadKGFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasThreadKGFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasToolResultKGFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasToolResultKGFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1326 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/HyperEdge_hasKGExtractionEdge.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/HyperEdge_hasKGExtractionEdge.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1572 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGActionStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGActionStatus.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGActionType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGActionType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1332 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGActor.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGActor.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1244 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGActorType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      106 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGActorType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     3340 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      746 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentPublishStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentPublishStatus.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1486 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentPublisher.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentPublisher.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentPublisherType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      115 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentPublisherType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentService.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentService.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2666 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentSubmission.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      581 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentSubmission.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1274 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentSubmissionType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      116 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentSubmissionType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1244 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      106 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1481 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAggregation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      178 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAggregation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1733 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAggregationResult.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      263 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAggregationResult.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAggregationType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAggregationType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1458 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAnnotation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAnnotation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1259 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAnnotationType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      111 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAnnotationType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1676 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAppEvent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAppEvent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAppEventSource.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAppEventSource.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAppEventType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAppEventType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1340 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAudio.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAudio.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1347 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAudioSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAudioSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGBeliefModeType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGBeliefModeType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1359 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGBooleanSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGBooleanSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1251 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGBracket.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      117 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGBracket.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1364 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCalendarEvent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCalendarEvent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1268 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCalendarEventType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      114 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCalendarEventType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1450 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCategory.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1253 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCategoryType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      109 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCategoryType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChatBotMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChatBotMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1613 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChatInteraction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChatInteraction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1274 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChatInteractionType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      116 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChatInteractionType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1908 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChatMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      304 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChatMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1262 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChatMessageType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      112 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChatMessageType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1283 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChatUserMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChatUserMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1379 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChoiceOptionSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChoiceOptionSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1354 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChoiceSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChoiceSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1799 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCodeDocument.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      263 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCodeDocument.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1265 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCodeDocumentType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      113 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCodeDocumentType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCodeLanguage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCodeLanguage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1343 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCodeSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCodeSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGConstraintComparator.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGConstraintComparator.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     4797 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCriterion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1208 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCriterion.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCriterionType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCriterionType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1362 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCurrencySlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCurrencySlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1364 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDateTimeSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDateTimeSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1481 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDescriptor.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      180 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDescriptor.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     3603 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDocument.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      837 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDocument.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDocumentSegmentMethod.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDocumentSegmentMethod.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDocumentSegmentType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDocumentSegmentType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1253 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDocumentType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      109 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDocumentType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1354 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDoubleSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDoubleSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2442 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEMail.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      452 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEMail.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1244 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEMailType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      106 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEMailType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGElement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      104 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGElement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1970 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEntity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      303 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEntity.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1892 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEntityMention.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      286 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEntityMention.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1351 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEntitySlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEntitySlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1247 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEntityType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      107 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEntityType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1332 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEvent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEvent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1244 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEventType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      106 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEventType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGExpressionType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGExpressionType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1353 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGExtractTask.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGExtractTask.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGExtractor.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGExtractor.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1449 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFigure.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFigure.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1340 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFileType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFileType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1367 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFileUploadSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFileUploadSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1753 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFlag.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      239 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFlag.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFlagReason.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFlagReason.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFlagSource.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFlagSource.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1241 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFlagType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      105 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFlagType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1253 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFormType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      118 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFormType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2274 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      380 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1477 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFrameProtoType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      169 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFrameProtoType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1362 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFrameType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFrameType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1392 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFrameTypeDescriptor.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFrameTypeDescriptor.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1379 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGGeoLocationSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGGeoLocationSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1332 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGGroup.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGGroup.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1244 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGGroupType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      106 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGGroupType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1454 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIPAddress.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIPAddress.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1446 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGImage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGImage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1347 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGImageSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGImageSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2956 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexDocument.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      647 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexDocument.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1985 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexDocumentAttempt.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      354 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexDocumentAttempt.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1320 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexDocumentAttemptStatusType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexDocumentAttemptStatusType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1311 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexDocumentClassification.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexDocumentClassification.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexDocumentStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexDocumentStatus.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1302 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexDocumentStorageType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexDocumentStorageType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexStatus.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1465 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGInstruction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGInstruction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1262 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGInstructionType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      112 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGInstructionType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1359 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIntegerSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIntegerSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1468 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGInteraction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGInteraction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1262 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGInteractionType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      112 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGInteractionType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1346 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGJSONSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGJSONSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1344 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGLongSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGLongSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1362 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGLongTextSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGLongTextSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1553 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGMedia.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      181 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGMedia.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1254 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGMetaType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      118 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGMetaType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1393 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGMultiChoiceOptionSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGMultiChoiceOptionSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1375 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGMultiChoiceSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGMultiChoiceSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGMultiTaxonomyOptionSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGMultiTaxonomyOptionSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1380 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGMultiTaxonomySlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGMultiTaxonomySlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1484 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGNewsEntity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      182 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGNewsEntity.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2544 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      493 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1364 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGNodeProxy.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGNodeProxy.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1584 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGNoteDocument.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGNoteDocument.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1265 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGNoteDocumentType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      113 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGNoteDocumentType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1360 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGOrganization.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGOrganization.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1265 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGOrganizationType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      113 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGOrganizationType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1242 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGPath.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      114 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGPath.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGPathElement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGPathElement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1547 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGPlace.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      178 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGPlace.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1563 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGPointer.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      196 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGPointer.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1262 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGProductEntity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      116 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGProductEntity.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1828 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGPropertySlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      295 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGPropertySlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGProvenanceType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGProvenanceType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1354 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQuery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQuery.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1274 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryANDGroup.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryANDGroup.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1322 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryCriteriaANDGroup.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryCriteriaANDGroup.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryCriteriaGroup.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryCriteriaGroup.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1319 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryCriteriaORGroup.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryCriteriaORGroup.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryExploreTraversal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryExploreTraversal.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryGroup.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryGroup.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryORGroup.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryORGroup.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1476 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQuerySort.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      180 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQuerySort.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQuerySortDirection.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQuerySortDirection.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQuerySortType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQuerySortType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryTraversal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryTraversal.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2098 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRating.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      350 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRating.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRatingSource.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRatingSource.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2654 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRatingSummary.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      584 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRatingSummary.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1268 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRatingSummaryType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      114 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRatingSummaryType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1247 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRatingType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      107 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRatingType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRatingValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRatingValue.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRatingValueType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRatingValueType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1368 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRelationType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRelationType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2150 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRelationTypeRestriction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      443 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRelationTypeRestriction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1349 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRequest.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRequest.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1250 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRequestType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      108 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRequestType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1563 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGResource.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      188 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGResource.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1253 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGResourceType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      109 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGResourceType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1454 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGResponse.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1253 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGResponseType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      109 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGResponseType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1463 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRunDocument.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRunDocument.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1262 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRunDocumentType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      112 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRunDocumentType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1339 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRunSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRunSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1446 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSearch.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSearch.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1247 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSearchType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      107 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSearchType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2178 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      360 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotConstraintType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotConstraintType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1472 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotProtoType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotProtoType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1252 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotRoleType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      109 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotRoleType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1385 2024-05-04 22:21:49.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotTypDescriptor.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 22:21:49.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotTypDescriptor.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1678 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1387 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotTypeDescriptor.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotTypeDescriptor.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotValueType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotValueType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1349 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGStatement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGStatement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2055 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGStatsSummary.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      364 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGStatsSummary.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1265 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGStatsSummaryType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      113 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGStatsSummaryType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1232 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTable.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      102 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTable.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1425 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTag.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTag.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTagType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      104 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTagType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1328 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTask.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      117 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTask.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1241 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTaskType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      105 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTaskType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1379 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTaxonomyOptionSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTaxonomyOptionSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1359 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTaxonomySlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTaxonomySlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1680 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTenant.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTenant.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1346 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTextSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTextSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1235 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGThread.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      103 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGThread.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1352 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGToolResult.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGToolResult.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1259 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGToolResultType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      111 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGToolResultType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1562 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      192 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1259 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTypeMethod.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTypeMethod.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     3229 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTypePath.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      656 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTypePath.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTypeRestriction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTypeRestriction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1339 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGURISlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGURISlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     3082 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGUserContext.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      700 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGUserContext.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGValidType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGValidType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1340 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGVideo.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGVideo.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1347 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGVideoSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGVideoSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1245 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGVisit.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      115 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGVisit.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1486 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGWebEntity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      183 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGWebEntity.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/NewsCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/NewsCategory.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/NewsContentCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/NewsContentCategory.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:39:48.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-18 22:40:37.674063 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasAnnotationText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasAudioSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasBooleanSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasChoiceSlotOptionValues.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasChoiceSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasCodeSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasCurrencySlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasDateTimeSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      262 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasDestinationRelationTypeRestrictionURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasDocumentAttemptDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasDocumentAttemptStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasDocumentAttemptStatusCode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasDocumentAuthorList.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasDocumentContentPath.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasDocumentContentType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasDocumentCorrectedURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasDocumentDescription.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasDocumentHTMLContent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasDocumentHeadline.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasDocumentOriginalURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasDocumentPublicationDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasDocumentRetrievalDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasDocumentURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasDocumentVersion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasDomainCategoryIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasDoubleSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasEdgeName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasEntitySlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasFileUploadSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasFrameGraphURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasFrameSequence.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasGeoLocationSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasHaleyRegionURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasImageSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasIntegerSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasInteractionSequence.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasJsonSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGActionAttemptDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGActionStatusURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGActionType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGActionTypeList.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGActionTypeSummaryDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGActorType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentAvatarImageSourceURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentAvatarImageURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentAvatarLargeImageURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentDeploymentURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentDescription.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentImplIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentModificationDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentNameSlug.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentPublishStatusURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentPublisherName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentPublisherType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentPublisherWebsiteURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentRankingScore.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      254 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentRankingScoreUpdateDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentServiceURIs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentSubmissionComments.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentSubmissionCreator.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentSubmissionDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentSubmissionDescription.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentSubmissionName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      250 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentSubmissionSubmitterEmail.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      248 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentSubmissionSubmitterName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentSubmissionType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentSubmissionURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAgentType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAggregationDoubleValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAggregationIntegerValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAggregationName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAggregationTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAnnotationType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAppEventActorURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAppEventAgent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAppEventSourceURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGAppEventType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGBeliefModeType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGBracketURIs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGCalendarEventType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGCategoryType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGChatInteractionCompleteText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGChatInteractionSummaryText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGChatInteractionType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGChatInteractionURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGChatMessageDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGChatMessageSequence.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGChatMessageText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGChatMessageType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGCodeDocumentType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGCodeInterpreterVersion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGCodeLanguageURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGCodeLanguageVersion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGConstraintComparatorURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGContentType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGCriterionTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGDataHash.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGDescriptorLabel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGDescriptorLanguageURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGDocumentContent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGDocumentDescription.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGDocumentEndTokenIndex.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGDocumentExtractedContent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGDocumentHTMLContent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGDocumentHeadline.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGDocumentPublicationDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGDocumentRetrievalDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGDocumentSegmentIndex.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGDocumentSegmentMethodURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGDocumentSegmentTokenLength.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGDocumentSegmentTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGDocumentStartTokenIndex.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGDocumentSummary.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGDocumentTokenLength.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGDocumentType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGDocumentURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGEMailType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGEmailBCCAddressList.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGEmailCCAddressList.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGEmailRecipientAddress.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGEmailRecipientName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGEmailSendDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGEmailSenderAddress.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGEmailSenderName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGEmailSubject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGEmailSummary.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGEmailToAddressList.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGEncodedByteData.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGEndByteIndex.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGEndTokenIndex.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGEntityAccountURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGEntityLoginURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGEntityType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGEntityTypeDescription.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGEventType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGExpressionType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGExtractTaskURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGExtractorURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGFileType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGFlagDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGFlagDescription.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGFlagReasonURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGFlagSourceURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGFlagType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGFormType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGFrameType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGFrameTypeDescription.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGFrameTypeExternIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGGraphAssertionDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGGroupType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGIPAddress.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGIPAddressJSON.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGIndexDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      258 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGIndexDocumentAttemptStatusTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGIndexDocumentClassificationURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGIndexDocumentStatusURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGIndexDocumentStorageTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGIndexStatusURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGInstructionText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGInstructionType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGInteractionType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGMediaDuration.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGMediaEncoding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGModelVersion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGNewsEntityBiasMetric.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGNewsEntityPrimaryDomain.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGNodeCacheDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGNodeReferenceURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGNoteDocumentContent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGNoteDocumentTitle.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGNoteDocumentType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGOrganizationType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGPixelHeight.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGPixelWidth.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGPlaceIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGPlaceJSON.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGPlaceURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGPointerNextURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGPointerPriorURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGPointerURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGPropertyGroupNameSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGPropertyNameSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGProvenanceType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryBooleanValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryChoiceValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryDateTimeValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryDoubleValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryIntegerValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryKGMetaType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryKGNodeClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryKGRelationType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryKGType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryLongTextValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryMoveFromConcepts.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryMoveToConcepts.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryMultiChoiceValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryMultiTaxonomyValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryNearVectorCertainty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryNearVectorDistance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryNearVectorForce.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryObjectURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryPropertyURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryProvenanceURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryRootURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQuerySerializedVector.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQuerySortDirectionURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQuerySortTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryTaxonomyValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryTextValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryTopKLimit.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryURIValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGQueryUnknownValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRatingCalculationDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRatingDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRatingDescription.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRatingSourceURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRatingStarValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      256 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRatingSummaryAverageRatingDouble.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRatingSummaryAverageStarRating.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRatingSummaryNegativeCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRatingSummaryNeutralCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRatingSummaryPositiveCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRatingSummaryReviewCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRatingSummaryText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRatingSummaryTitle.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRatingSummaryTotalCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRatingSummaryType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRatingType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRatingValueDouble.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRatingValueTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRatingValueURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRelationType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRelationTypeDescription.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRelationTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRequestType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRequestURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGResourceDescription.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGResourceName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGResourceType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGResponseType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRunCodeOutput.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGRunDocumentType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGSearchDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGSearchType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGSlotConstraintType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGSlotReferenceURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGSlotRoleSequence.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGSlotRoleType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGSlotType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGSlotTypeClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGSlotTypeDescription.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGSlotTypeExternIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGSlotTypeLabel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGSlotTypeName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGSlotValueType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGSourceCode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGStartByteIndex.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGStartTokenIndex.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGStatsSummaryCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGStatsSummaryCountPercentage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGStatsSummaryPeriod.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGStatsSummaryPeriodDay.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGStatsSummaryPeriodMonth.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGStatsSummaryPeriodYear.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGStatsSummaryType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGTagName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGTagType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGTaskType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGTaxonomyOptionURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGTenantAccountID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGTenantAccountURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGTenantIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGToolResultType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGTypeClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGTypeMethodURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGTypeVersion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGUserContextAccountLevel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGUserContextAccountURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGUserContextAgentFamiliarity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGUserContextAgentTone.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGUserContextCurrentDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGUserContextCurrentTimezone.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGUserContextExperienceLevel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGUserContextGender.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGUserContextLightLevel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGUserContextLocation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGUserContextLoginURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGUserContextMood.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGUserContextName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGUserContextPronoun.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGUserContextSoundLevel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGValidTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGVersion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGWebEntityDomainCategories.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGWebEntityPrimaryDomain.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasKGraphDescription.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasLongSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasLongTextSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasMultiChoiceSlotValues.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasMultiTaxonomySlotValues.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasParentFrameURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasPrimaryLanguageType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasPropertyClassSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasPropertyFrameTypeSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasPropertySlotTypeSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasRunSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasSlotSequence.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasSourceRelationTypeRestrictionURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasStatementText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasTaxonomySlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasTextSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasTopCategoryURIs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasUnionDomainBooleanProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasUnionDomainDateTimeProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasUnionDomainDoubleProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasUnionDomainFloatProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasUnionDomainIntegerProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasUnionDomainLongProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasUnionDomainObjectProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasUnionDomainStringProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasUriSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_hasVideoSlotValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_isKGAgentSubmissionApproved.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_isKGAgentSubmissionConverted.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_isKGAgentSubmissionReviewed.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_isKGCategoryRoot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_isKGGlobalTenant.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_isKGQuerySubclassExpansion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_isKGQuerySubtypeExpansion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_isKGRelationTypeDestinationOpen.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      248 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_isKGRelationTypeExpandDestination.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_isKGRelationTypeExpandSource.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_isKGRelationTypeSourceOpen.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-18 22:25:02.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/Property_isKGRelationTypeSymmetric.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:39:48.000000 vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/properties/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-18 22:40:37.675915 vital-ai-haley-kg-0.1.6/setup.cfg
+-rw-r--r--   0 hadfield   (501) staff       (20)      896 2024-05-18 22:25:38.000000 vital-ai-haley-kg-0.1.6/setup.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-18 22:40:37.675062 vital-ai-haley-kg-0.1.6/vital_ai_haley_kg.egg-info/
+-rw-r--r--   0 hadfield   (501) staff       (20)      501 2024-05-18 22:40:37.000000 vital-ai-haley-kg-0.1.6/vital_ai_haley_kg.egg-info/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)    50425 2024-05-18 22:40:37.000000 vital-ai-haley-kg-0.1.6/vital_ai_haley_kg.egg-info/SOURCES.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-18 22:40:37.000000 vital-ai-haley-kg-0.1.6/vital_ai_haley_kg.egg-info/dependency_links.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       62 2024-05-18 22:40:37.000000 vital-ai-haley-kg-0.1.6/vital_ai_haley_kg.egg-info/entry_points.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       31 2024-05-18 22:40:37.000000 vital-ai-haley-kg-0.1.6/vital_ai_haley_kg.egg-info/requires.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       19 2024-05-18 22:40:37.000000 vital-ai-haley-kg-0.1.6/vital_ai_haley_kg.egg-info/top_level.txt
```

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/DomainCategory.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/DomainCategory.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasActorKGFrame.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasActorKGFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasAgentKGFrame.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasAgentKGFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasChatMessageKGFrame.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasChatMessageKGFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasDocumentKGFrame.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasDocumentKGFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasEntityKGFrame.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasEntityKGFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasEntityKGStatement.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasEntityKGStatement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasEntityTypePartOfKGFrameType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasEntityTypePartOfKGFrameType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasEventKGFrame.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasEventKGFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasGroupKGFrame.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasGroupKGFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasIncomingKGRelationType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasIncomingKGRelationType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasInteractionKGDocument.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasInteractionKGDocument.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasInteractionKGEntity.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasInteractionKGEntity.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasInteractionKGFrame.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasInteractionKGFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGAction.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGActor.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGActor.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGAgent.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGAgent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGAgentDuplicate.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGAgentDuplicate.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGAgentPublisher.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGAgentPublisher.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGAggregation.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGAggregation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGAnnotation.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGAnnotation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGBroadCategory.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGBroadCategory.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGCategory.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGCategory.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGChatMessage.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGChatMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGCriterion.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGCriterion.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGDocument.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGDocument.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGDocumentFileNode.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGDocumentFileNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGDocumentSegment.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGDocumentSegment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGEdge.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGEdge.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGEntity.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGEntity.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGEntityMention.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGEntityMention.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGExtractTask.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGExtractTask.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGExtraction.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGExtraction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGFigure.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGFigure.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGFlag.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGFlag.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGFrame.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGGroup.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGGroup.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGIndexDocumentAttempt.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGIndexDocumentAttempt.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGIndexDocumentCategory.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGIndexDocumentCategory.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGIndexDocumentFileNode.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGIndexDocumentFileNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGInstruction.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGInstruction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGInteractionDependency.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGInteractionDependency.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGInteractionElement.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGInteractionElement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGMedia.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGMedia.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGMediaFileNode.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGMediaFileNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGNarrowCategory.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGNarrowCategory.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGNode.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGNormalizedEntity.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGNormalizedEntity.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGOrganization.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGOrganization.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGPath.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGPath.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGPathElement.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGPathElement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGPointer.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGPointer.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGQueryCriteriaGroup.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGQueryCriteriaGroup.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGQueryExploreTraversal.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGQueryExploreTraversal.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGQueryGroup.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGQueryGroup.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGQuerySort.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGQuerySort.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGQueryTraversal.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGQueryTraversal.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRating.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRating.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRatingSummary.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRatingSummary.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRefEdge.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRefEdge.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRefRelation.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRefRelation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRelation.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRelation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRelationMention.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRelationMention.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGResource.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGResource.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGRunDocument.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGRunDocument.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGSearch.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGSearch.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGSlotProtoType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGSlotProtoType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGSlotType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGSlotType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGStatement.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGStatement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGStatsSummary.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGStatsSummary.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGTable.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGTable.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGTag.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGTag.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGThread.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGThread.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasKGTypePath.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasKGTypePath.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasOrganizationKGFrame.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasOrganizationKGFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasOutgoingKGRelationType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasOutgoingKGRelationType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasPartOfKGFrameType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasPartOfKGFrameType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasRecipientEntityKGEmail.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasRecipientEntityKGEmail.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasRequestKGFrame.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasRequestKGFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasResourceKGFrame.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasResourceKGFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasResponseKGFrame.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasResponseKGFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasRunKGFrame.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasRunKGFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSameAsKGEntity.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSameAsKGEntity.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSameAsKGEntityMention.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSameAsKGEntityMention.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSameAsKGType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSameAsKGType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSearchKGEntityMention.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSearchKGEntityMention.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSenderEntityKGEmail.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSenderEntityKGEmail.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSubKGFrameType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSubKGFrameType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasSubKGType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasSubKGType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasTableKGFrame.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasTableKGFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasTaskKGFrame.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasTaskKGFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasThreadKGFrame.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasThreadKGFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/Edge_hasToolResultKGFrame.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/Edge_hasToolResultKGFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/HyperEdge_hasKGExtractionEdge.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/HyperEdge_hasKGExtractionEdge.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAction.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGActionStatus.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGActionStatus.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGActionType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGActionType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGActor.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGActor.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGActorType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGActorType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgent.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgent.pyi` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgent.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentPublishStatus.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentPublishStatus.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentPublisher.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentPublisher.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentPublisherType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentPublisherType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentService.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentService.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentSubmission.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentSubmission.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentSubmission.pyi` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentSubmission.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentSubmissionType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentSubmissionType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAgentType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAgentType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAggregation.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAggregation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAggregationResult.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAggregationResult.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAggregationType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAggregationType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAnnotation.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAnnotation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAnnotationType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAnnotationType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAppEvent.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAppEvent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAppEventSource.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAppEventSource.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAppEventType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAppEventType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAudio.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAudio.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGAudioSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGAudioSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGBeliefModeType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGBeliefModeType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGBooleanSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGBooleanSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGBracket.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGBracket.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCalendarEvent.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCalendarEvent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCalendarEventType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCalendarEventType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCategory.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCategory.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCategoryType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCategoryType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChatBotMessage.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChatBotMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChatInteraction.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChatInteraction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChatInteractionType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChatInteractionType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChatMessage.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChatMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChatMessageType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChatMessageType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChatUserMessage.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChatUserMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChoiceOptionSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChoiceOptionSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGChoiceSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGChoiceSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCodeDocument.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCodeDocument.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCodeDocumentType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCodeDocumentType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCodeLanguage.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCodeLanguage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCodeSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCodeSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGConstraintComparator.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGConstraintComparator.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCriterion.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCriterion.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCriterion.pyi` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCriterion.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCriterionType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCriterionType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGCurrencySlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGCurrencySlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDateTimeSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDateTimeSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDescriptor.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDescriptor.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDocument.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDocument.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDocument.pyi` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDocument.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDocumentSegmentMethod.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDocumentSegmentMethod.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDocumentSegmentType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDocumentSegmentType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDocumentType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDocumentType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGDoubleSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGDoubleSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEMail.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEMail.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEMailType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEMailType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGElement.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGElement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEntity.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEntity.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEntityMention.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEntityMention.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEntitySlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEntitySlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEntityType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEntityType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEvent.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEvent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGEventType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGEventType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGExpressionType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGExpressionType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGExtractTask.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGExtractTask.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGExtractor.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGExtractor.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFigure.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFigure.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFileType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFileType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFileUploadSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFileUploadSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFlag.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFlag.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFlagReason.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFlagReason.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFlagSource.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFlagSource.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFlagType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFlagType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFormType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFormType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFrame.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFrameProtoType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFrameProtoType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFrameType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFrameType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGFrameTypeDescriptor.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGFrameTypeDescriptor.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGGeoLocationSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGGeoLocationSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGGroup.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGGroup.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGGroupType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGGroupType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIPAddress.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIPAddress.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGImage.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGImage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGImageSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGImageSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexDocument.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexDocument.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexDocument.pyi` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexDocument.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexDocumentAttempt.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexDocumentAttempt.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexDocumentAttemptStatusType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexDocumentAttemptStatusType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexDocumentClassification.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexDocumentClassification.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexDocumentStatus.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexDocumentStatus.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexDocumentStorageType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexDocumentStorageType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIndexStatus.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIndexStatus.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGInstruction.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGInstruction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGInstructionType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGInstructionType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGIntegerSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGIntegerSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGInteraction.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGInteraction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGInteractionType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGInteractionType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGJSONSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGJSONSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGLongSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGLongSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGLongTextSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGLongTextSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGMedia.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGMedia.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGMetaType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGMetaType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGMultiChoiceOptionSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGMultiChoiceOptionSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGMultiChoiceSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGMultiChoiceSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGMultiTaxonomyOptionSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGMultiTaxonomyOptionSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGMultiTaxonomySlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGMultiTaxonomySlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGNewsEntity.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGNewsEntity.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGNode.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGNodeProxy.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGNodeProxy.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGNoteDocument.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGNoteDocument.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGNoteDocumentType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGNoteDocumentType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGOrganization.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGOrganization.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGOrganizationType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGOrganizationType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGPath.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGPath.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGPathElement.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGPathElement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGPlace.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGPlace.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGPointer.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGPointer.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGProductEntity.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGProductEntity.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGPropertySlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGPropertySlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGProvenanceType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGProvenanceType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQuery.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQuery.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryANDGroup.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryANDGroup.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryCriteriaANDGroup.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryCriteriaANDGroup.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryCriteriaGroup.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryCriteriaGroup.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryCriteriaORGroup.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryCriteriaORGroup.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryExploreTraversal.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryExploreTraversal.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryGroup.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryGroup.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryORGroup.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryORGroup.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQuerySort.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQuerySort.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQuerySortDirection.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQuerySortDirection.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQuerySortType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQuerySortType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGQueryTraversal.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGQueryTraversal.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRating.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRating.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRatingSource.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRatingSource.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRatingSummary.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRatingSummary.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRatingSummary.pyi` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRatingSummary.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRatingSummaryType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRatingSummaryType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRatingType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRatingType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRatingValue.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRatingValue.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRatingValueType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRatingValueType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRelationType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRelationType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRelationTypeRestriction.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRelationTypeRestriction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRequest.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRequest.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRequestType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRequestType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGResource.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGResource.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGResourceType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGResourceType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGResponse.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGResponse.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGResponseType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGResponseType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRunDocument.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRunDocument.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRunDocumentType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRunDocumentType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGRunSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGRunSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSearch.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSearch.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSearchType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSearchType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotConstraintType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotConstraintType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotProtoType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotProtoType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotRoleType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotRoleType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotTypDescriptor.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotTypDescriptor.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotTypeDescriptor.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotTypeDescriptor.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGSlotValueType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGSlotValueType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGStatement.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGStatement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGStatsSummary.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGStatsSummary.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGStatsSummaryType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGStatsSummaryType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTable.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTable.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTag.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTag.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTagType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTagType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTask.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTask.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTaskType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTaskType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTaxonomyOptionSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTaxonomyOptionSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTaxonomySlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTaxonomySlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTenant.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTenant.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTextSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTextSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGThread.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGThread.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGToolResult.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGToolResult.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGToolResultType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGToolResultType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTypeMethod.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTypeMethod.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTypePath.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTypePath.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTypePath.pyi` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTypePath.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGTypeRestriction.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGTypeRestriction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGURISlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGURISlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGUserContext.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGUserContext.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGUserContext.pyi` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGUserContext.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGValidType.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGValidType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGVideo.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGVideo.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGVideoSlot.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGVideoSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGVisit.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGVisit.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/KGWebEntity.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/KGWebEntity.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/NewsCategory.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/NewsCategory.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/ai_haley_kg_domain/model/NewsContentCategory.py` & `vital-ai-haley-kg-0.1.6/ai_haley_kg_domain/model/NewsContentCategory.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-kg-0.1.5/setup.py` & `vital-ai-haley-kg-0.1.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vital-ai-haley-kg',
-    version='0.1.5',
+    version='0.1.6',
     author='Marc Hadfield',
     author_email='marc@vital.ai',
     description='VitalSigns haley kg domain',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vital-ai/vitalhome-haley',
     packages=find_packages(),
```

### Comparing `vital-ai-haley-kg-0.1.5/vital_ai_haley_kg.egg-info/SOURCES.txt` & `vital-ai-haley-kg-0.1.6/vital_ai_haley_kg.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 ai_haley_kg_domain/model/Edge_hasKGAggregation.pyi
 ai_haley_kg_domain/model/Edge_hasKGAnnotation.py
 ai_haley_kg_domain/model/Edge_hasKGAnnotation.pyi
 ai_haley_kg_domain/model/Edge_hasKGBroadCategory.py
 ai_haley_kg_domain/model/Edge_hasKGBroadCategory.pyi
 ai_haley_kg_domain/model/Edge_hasKGCategory.py
 ai_haley_kg_domain/model/Edge_hasKGCategory.pyi
+ai_haley_kg_domain/model/Edge_hasKGChatInteraction.py
+ai_haley_kg_domain/model/Edge_hasKGChatInteraction.pyi
 ai_haley_kg_domain/model/Edge_hasKGChatMessage.py
 ai_haley_kg_domain/model/Edge_hasKGChatMessage.pyi
 ai_haley_kg_domain/model/Edge_hasKGCriterion.py
 ai_haley_kg_domain/model/Edge_hasKGCriterion.pyi
 ai_haley_kg_domain/model/Edge_hasKGDocument.py
 ai_haley_kg_domain/model/Edge_hasKGDocument.pyi
 ai_haley_kg_domain/model/Edge_hasKGDocumentFileNode.py
@@ -878,14 +880,22 @@
 ai_haley_kg_domain/model/properties/Property_hasRunSlotValue.py
 ai_haley_kg_domain/model/properties/Property_hasSlotSequence.py
 ai_haley_kg_domain/model/properties/Property_hasSourceRelationTypeRestrictionURI.py
 ai_haley_kg_domain/model/properties/Property_hasStatementText.py
 ai_haley_kg_domain/model/properties/Property_hasTaxonomySlotValue.py
 ai_haley_kg_domain/model/properties/Property_hasTextSlotValue.py
 ai_haley_kg_domain/model/properties/Property_hasTopCategoryURIs.py
+ai_haley_kg_domain/model/properties/Property_hasUnionDomainBooleanProperty.py
+ai_haley_kg_domain/model/properties/Property_hasUnionDomainDateTimeProperty.py
+ai_haley_kg_domain/model/properties/Property_hasUnionDomainDoubleProperty.py
+ai_haley_kg_domain/model/properties/Property_hasUnionDomainFloatProperty.py
+ai_haley_kg_domain/model/properties/Property_hasUnionDomainIntegerProperty.py
+ai_haley_kg_domain/model/properties/Property_hasUnionDomainLongProperty.py
+ai_haley_kg_domain/model/properties/Property_hasUnionDomainObjectProperty.py
+ai_haley_kg_domain/model/properties/Property_hasUnionDomainStringProperty.py
 ai_haley_kg_domain/model/properties/Property_hasUriSlotValue.py
 ai_haley_kg_domain/model/properties/Property_hasVideoSlotValue.py
 ai_haley_kg_domain/model/properties/Property_isKGAgentSubmissionApproved.py
 ai_haley_kg_domain/model/properties/Property_isKGAgentSubmissionConverted.py
 ai_haley_kg_domain/model/properties/Property_isKGAgentSubmissionReviewed.py
 ai_haley_kg_domain/model/properties/Property_isKGCategoryRoot.py
 ai_haley_kg_domain/model/properties/Property_isKGGlobalTenant.py
```

