# Comparing `tmp/stigg_api_client_v2-0.522.0.tar.gz` & `tmp/stigg_api_client_v2-0.523.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.522.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.523.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.522.0.tar` & `stigg_api_client_v2-0.523.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1644 2023-08-03 12:58:37.846175 stigg_api_client_v2-0.522.0/README.md
--rw-r--r--   0        0        0      452 2023-08-03 12:59:36.334378 stigg_api_client_v2-0.522.0/pyproject.toml
--rw-r--r--   0        0        0       62 2023-08-03 12:58:37.846175 stigg_api_client_v2-0.522.0/stigg/__init__.py
--rw-r--r--   0        0        0     4711 2023-08-03 12:58:37.846175 stigg_api_client_v2-0.522.0/stigg/client.py
--rw-r--r--   0        0        0      932 2023-08-03 12:58:37.846175 stigg_api_client_v2-0.522.0/stigg/edge_utils.py
--rw-r--r--   0        0        0    41178 2023-08-03 12:59:34.242369 stigg_api_client_v2-0.522.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0      460 2023-08-03 12:59:32.490362 stigg_api_client_v2-0.522.0/stigg/generated/archive_customer.py
--rw-r--r--   0        0        0     7303 2023-08-03 12:59:33.638367 stigg_api_client_v2-0.522.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0    70891 2023-08-03 12:59:34.038368 stigg_api_client_v2-0.522.0/stigg/generated/async_client.py
--rw-r--r--   0        0        0     2731 2023-08-03 12:59:27.218340 stigg_api_client_v2-0.522.0/stigg/generated/base_client.py
--rw-r--r--   0        0        0     1951 2023-08-03 12:59:33.638367 stigg_api_client_v2-0.522.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-08-03 12:59:32.418362 stigg_api_client_v2-0.522.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-08-03 12:59:32.442362 stigg_api_client_v2-0.522.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    70464 2023-08-03 12:59:27.478341 stigg_api_client_v2-0.522.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-08-03 12:59:32.474362 stigg_api_client_v2-0.522.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0    24514 2023-08-03 12:59:29.422349 stigg_api_client_v2-0.522.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-08-03 12:59:32.430362 stigg_api_client_v2-0.522.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-08-03 12:59:32.438362 stigg_api_client_v2-0.522.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-08-03 12:59:33.638367 stigg_api_client_v2-0.522.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    58974 2023-08-03 12:59:33.638367 stigg_api_client_v2-0.522.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-08-03 12:59:32.506362 stigg_api_client_v2-0.522.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-08-03 12:59:32.518362 stigg_api_client_v2-0.522.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-08-03 12:59:32.498362 stigg_api_client_v2-0.522.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-08-03 12:59:32.562362 stigg_api_client_v2-0.522.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-08-03 12:59:32.534362 stigg_api_client_v2-0.522.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-08-03 12:59:32.530362 stigg_api_client_v2-0.522.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-08-03 12:59:32.574362 stigg_api_client_v2-0.522.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-08-03 12:59:32.522362 stigg_api_client_v2-0.522.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-08-03 12:59:32.546362 stigg_api_client_v2-0.522.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-08-03 12:59:32.558362 stigg_api_client_v2-0.522.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-08-03 12:59:32.382361 stigg_api_client_v2-0.522.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-08-03 12:59:32.374361 stigg_api_client_v2-0.522.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-08-03 12:59:32.406361 stigg_api_client_v2-0.522.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   128817 2023-08-03 12:59:32.350361 stigg_api_client_v2-0.522.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-08-03 12:59:32.482362 stigg_api_client_v2-0.522.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-08-03 12:59:32.366361 stigg_api_client_v2-0.522.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-08-03 12:59:32.402361 stigg_api_client_v2-0.522.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-08-03 12:59:32.466362 stigg_api_client_v2-0.522.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-08-03 12:59:32.458362 stigg_api_client_v2-0.522.0/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-08-03 12:59:32.450362 stigg_api_client_v2-0.522.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-08-03 12:59:33.646366 stigg_api_client_v2-0.522.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-08-03 12:59:32.390361 stigg_api_client_v2-0.522.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-08-03 12:59:32.414362 stigg_api_client_v2-0.522.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-08-03 12:59:32.582362 stigg_api_client_v2-0.522.0/stigg/generated/usage_history.py
--rw-r--r--   0        0        0     2075 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.522.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-08-05 17:43:57.997593 stigg_api_client_v2-0.523.0/README.md
+-rw-r--r--   0        0        0      452 2023-08-05 17:44:51.146597 stigg_api_client_v2-0.523.0/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-08-05 17:43:57.997593 stigg_api_client_v2-0.523.0/stigg/__init__.py
+-rw-r--r--   0        0        0     4711 2023-08-05 17:43:57.997593 stigg_api_client_v2-0.523.0/stigg/client.py
+-rw-r--r--   0        0        0      932 2023-08-05 17:43:57.997593 stigg_api_client_v2-0.523.0/stigg/edge_utils.py
+-rw-r--r--   0        0        0    41178 2023-08-05 17:44:49.226565 stigg_api_client_v2-0.523.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0      460 2023-08-05 17:44:47.634538 stigg_api_client_v2-0.523.0/stigg/generated/archive_customer.py
+-rw-r--r--   0        0        0     7303 2023-08-05 17:44:48.646555 stigg_api_client_v2-0.523.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0    70891 2023-08-05 17:44:49.034561 stigg_api_client_v2-0.523.0/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     2731 2023-08-05 17:44:42.838449 stigg_api_client_v2-0.523.0/stigg/generated/base_client.py
+-rw-r--r--   0        0        0     1951 2023-08-05 17:44:48.646555 stigg_api_client_v2-0.523.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-08-05 17:44:47.570537 stigg_api_client_v2-0.523.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-08-05 17:44:47.590537 stigg_api_client_v2-0.523.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    70464 2023-08-05 17:44:43.094454 stigg_api_client_v2-0.523.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-08-05 17:44:47.618538 stigg_api_client_v2-0.523.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0    24514 2023-08-05 17:44:44.930489 stigg_api_client_v2-0.523.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-08-05 17:44:47.578537 stigg_api_client_v2-0.523.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-08-05 17:44:47.586537 stigg_api_client_v2-0.523.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-08-05 17:44:48.646555 stigg_api_client_v2-0.523.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    58974 2023-08-05 17:44:48.646555 stigg_api_client_v2-0.523.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-08-05 17:44:47.650538 stigg_api_client_v2-0.523.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-08-05 17:44:47.662538 stigg_api_client_v2-0.523.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-08-05 17:44:47.642538 stigg_api_client_v2-0.523.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-08-05 17:44:47.706539 stigg_api_client_v2-0.523.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-08-05 17:44:47.678538 stigg_api_client_v2-0.523.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-08-05 17:44:47.674538 stigg_api_client_v2-0.523.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-08-05 17:44:47.718539 stigg_api_client_v2-0.523.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-08-05 17:44:47.666538 stigg_api_client_v2-0.523.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-08-05 17:44:47.686539 stigg_api_client_v2-0.523.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-08-05 17:44:47.698539 stigg_api_client_v2-0.523.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-08-05 17:44:47.530536 stigg_api_client_v2-0.523.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-08-05 17:44:47.526536 stigg_api_client_v2-0.523.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-08-05 17:44:47.554536 stigg_api_client_v2-0.523.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   128817 2023-08-05 17:44:47.506536 stigg_api_client_v2-0.523.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-08-05 17:44:47.626538 stigg_api_client_v2-0.523.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-08-05 17:44:47.518536 stigg_api_client_v2-0.523.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-08-05 17:44:47.550536 stigg_api_client_v2-0.523.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-08-05 17:44:47.610537 stigg_api_client_v2-0.523.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-08-05 17:44:47.606537 stigg_api_client_v2-0.523.0/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-08-05 17:44:47.598537 stigg_api_client_v2-0.523.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-08-05 17:44:48.654555 stigg_api_client_v2-0.523.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-08-05 17:44:47.538536 stigg_api_client_v2-0.523.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-08-05 17:44:47.562537 stigg_api_client_v2-0.523.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-08-05 17:44:47.722539 stigg_api_client_v2-0.523.0/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0     2075 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.523.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.522.0/README.md` & `stigg_api_client_v2-0.523.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.522.0/stigg/client.py` & `stigg_api_client_v2-0.523.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.522.0/stigg/edge_utils.py` & `stigg_api_client_v2-0.523.0/stigg/edge_utils.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.523.0/stigg/generated/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 
 from .archive_customer import ArchiveCustomer, ArchiveCustomerArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .async_client import AsyncClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.523.0/stigg/generated/async_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/async_client.py` & `stigg_api_client_v2-0.523.0/stigg/generated/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/base_client.py` & `stigg_api_client_v2-0.523.0/stigg/generated/base_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 
 import json
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.523.0/stigg/generated/base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.523.0/stigg/generated/cancel_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/client.py` & `stigg_api_client_v2-0.523.0/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .base_client import BaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.523.0/stigg/generated/create_subscription.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.523.0/stigg/generated/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerIsArchived = "CustomerIsArchived"
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.523.0/stigg/generated/estimate_subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.523.0/stigg/generated/estimate_subscription_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.523.0/stigg/generated/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.523.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -32,36 +32,14 @@
     VendorIdentifier,
     WeeklyAccordingTo,
     WidgetType,
     experimentGroupType,
 )
 
 
-class PackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    feature_id: str = Field(alias="featureId")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    is_custom: Optional[bool] = Field(alias="isCustom")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: "PackageEntitlementFragmentFeature"
-
-
-class PackageEntitlementFragmentFeature(BaseModel):
-    feature_type: FeatureType = Field(alias="featureType")
-    meter_type: Optional[MeterType] = Field(alias="meterType")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-    display_name: str = Field(alias="displayName")
-    description: Optional[str]
-    ref_id: str = Field(alias="refId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class PriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -78,14 +56,36 @@
     ref_id: str = Field(alias="refId")
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
 
 
+class PackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    feature_id: str = Field(alias="featureId")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    is_custom: Optional[bool] = Field(alias="isCustom")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: "PackageEntitlementFragmentFeature"
+
+
+class PackageEntitlementFragmentFeature(BaseModel):
+    feature_type: FeatureType = Field(alias="featureType")
+    meter_type: Optional[MeterType] = Field(alias="meterType")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+    ref_id: str = Field(alias="refId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class AddonFragment(BaseModel):
     id: str
     ref_id: str = Field(alias="refId")
     billing_id: Optional[str] = Field(alias="billingId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
@@ -329,25 +329,19 @@
     weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
 
 
 class CustomerPortalEntitlementFeature(FeatureFragment):
     pass
 
 
-class CustomerPortalPromotionalEntitlement(BaseModel):
+class CustomerPortalSubscriptionAddon(BaseModel):
+    addon_id: str = Field(alias="addonId")
+    description: Optional[str]
     display_name: str = Field(alias="displayName")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    period: PromotionalEntitlementPeriod
-    start_date: Any = Field(alias="startDate")
-    end_date: Optional[Any] = Field(alias="endDate")
-
-
-class CustomerResourceFragment(BaseModel):
-    resource_id: str = Field(alias="resourceId")
+    quantity: int
 
 
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
@@ -394,21 +388,14 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
-class CustomerPortalSubscriptionAddon(BaseModel):
-    addon_id: str = Field(alias="addonId")
-    description: Optional[str]
-    display_name: str = Field(alias="displayName")
-    quantity: int
-
-
 class CustomerPortalSubscriptionPriceFragment(BaseModel):
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
     billing_model: Optional[BillingModel] = Field(alias="billingModel")
     price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
     feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
 
 
@@ -506,14 +493,27 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateData
 ):
     pass
 
 
+class CustomerResourceFragment(BaseModel):
+    resource_id: str = Field(alias="resourceId")
+
+
+class CustomerPortalPromotionalEntitlement(BaseModel):
+    display_name: str = Field(alias="displayName")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    period: PromotionalEntitlementPeriod
+    start_date: Any = Field(alias="startDate")
+    end_date: Optional[Any] = Field(alias="endDate")
+
+
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
     ] = Field(alias="promotionalEntitlements")
     billing_information: "CustomerPortalFragmentBillingInformation" = Field(
@@ -621,127 +621,127 @@
 
 
 class PlanFragmentDefaultTrialConfig(BaseModel):
     duration: float
     units: TrialPeriodUnits
 
 
-class SubscriptionFutureUpdateData(BaseModel):
+class SubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
-    target_package: Optional["SubscriptionFutureUpdateDataTargetPackage"] = Field(
+    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
         alias="targetPackage"
     )
     schedule_variables: Optional[
         Annotated[
             Union[
-                "SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables",
-                "SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables",
-                "SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
             ],
             Field(discriminator="typename__"),
         ]
     ] = Field(alias="scheduleVariables")
 
 
-class SubscriptionFutureUpdateDataTargetPackage(BaseModel):
+class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
     id: str
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
 
 
-class SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables(
+class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
     BaseModel
 ):
     typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
 
 
-class SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables(BaseModel):
+class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
+    BaseModel
+):
     typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
     addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
     downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
 
 
-class SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables(BaseModel):
+class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
+    BaseModel
+):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
-class TotalPriceFragment(BaseModel):
-    sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
-    total: "TotalPriceFragmentTotal"
-
-
-class TotalPriceFragmentSubTotal(BaseModel):
-    amount: float
-    currency: Currency
-
-
-class TotalPriceFragmentTotal(BaseModel):
-    amount: float
-    currency: Currency
-
-
-class SubscriptionScheduledUpdateData(BaseModel):
+class SubscriptionFutureUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
-    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
+    target_package: Optional["SubscriptionFutureUpdateDataTargetPackage"] = Field(
         alias="targetPackage"
     )
     schedule_variables: Optional[
         Annotated[
             Union[
-                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
+                "SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables",
+                "SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables",
+                "SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables",
             ],
             Field(discriminator="typename__"),
         ]
     ] = Field(alias="scheduleVariables")
 
 
-class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
+class SubscriptionFutureUpdateDataTargetPackage(BaseModel):
     id: str
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
 
 
-class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
+class SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables(
     BaseModel
 ):
     typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
 
 
-class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
-    BaseModel
-):
+class SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables(BaseModel):
     typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
     addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
     downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
 
 
-class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
-    BaseModel
-):
+class SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables(BaseModel):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
+class TotalPriceFragment(BaseModel):
+    sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
+    total: "TotalPriceFragmentTotal"
+
+
+class TotalPriceFragmentSubTotal(BaseModel):
+    amount: float
+    currency: Currency
+
+
+class TotalPriceFragmentTotal(BaseModel):
+    amount: float
+    currency: Currency
+
+
 class SubscriptionFragment(BaseModel):
     id: str
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
     trial_end_date: Optional[Any] = Field(alias="trialEndDate")
     cancellation_date: Optional[Any] = Field(alias="cancellationDate")
     effective_end_date: Optional[Any] = Field(alias="effectiveEndDate")
@@ -899,14 +899,34 @@
 class LayoutConfigurationFragment(BaseModel):
     alignment: Optional[Alignment]
     plan_width: Optional[float] = Field(alias="planWidth")
     plan_margin: Optional[float] = Field(alias="planMargin")
     plan_padding: Optional[float] = Field(alias="planPadding")
 
 
+class MockPaywallPackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: Optional["MockPaywallPackageEntitlementFragmentFeature"]
+
+
+class MockPaywallPackageEntitlementFragmentFeature(BaseModel):
+    feature_type: FeatureType = Field(alias="featureType")
+    meter_type: Optional[MeterType] = Field(alias="meterType")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+    ref_id: str = Field(alias="refId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class MockPaywallPriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -922,34 +942,14 @@
 class MockPaywallPriceFragmentFeature(BaseModel):
     ref_id: str = Field(alias="refId")
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
 
 
-class MockPaywallPackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: Optional["MockPaywallPackageEntitlementFragmentFeature"]
-
-
-class MockPaywallPackageEntitlementFragmentFeature(BaseModel):
-    feature_type: FeatureType = Field(alias="featureType")
-    meter_type: Optional[MeterType] = Field(alias="meterType")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-    display_name: str = Field(alias="displayName")
-    description: Optional[str]
-    ref_id: str = Field(alias="refId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class MockPaywallAddonFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     billing_id: Optional[str] = Field(alias="billingId")
     entitlements: List["MockPaywallAddonFragmentEntitlements"]
@@ -1396,19 +1396,19 @@
 
 class UsageHistoryFragmentUsageMeasurements(BaseModel):
     date: Any
     value: float
     is_reset_point: Optional[bool] = Field(alias="isResetPoint")
 
 
-PackageEntitlementFragment.update_forward_refs()
-PackageEntitlementFragmentFeature.update_forward_refs()
 PriceFragment.update_forward_refs()
 PriceFragmentPrice.update_forward_refs()
 PriceFragmentFeature.update_forward_refs()
+PackageEntitlementFragment.update_forward_refs()
+PackageEntitlementFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
 SlimCustomerFragment.update_forward_refs()
@@ -1431,22 +1431,20 @@
 CustomerPortalConfigurationFragmentPalette.update_forward_refs()
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
-CustomerPortalPromotionalEntitlement.update_forward_refs()
-CustomerResourceFragment.update_forward_refs()
+CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
-CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionPriceFragment.update_forward_refs()
 CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
 CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPrices.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricing.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingPrice.update_forward_refs()
@@ -1454,14 +1452,16 @@
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
+CustomerResourceFragment.update_forward_refs()
+CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
@@ -1472,27 +1472,27 @@
 PlanFragmentProduct.update_forward_refs()
 PlanFragmentBasePlan.update_forward_refs()
 PlanFragmentEntitlements.update_forward_refs()
 PlanFragmentInheritedEntitlements.update_forward_refs()
 PlanFragmentCompatibleAddons.update_forward_refs()
 PlanFragmentPrices.update_forward_refs()
 PlanFragmentDefaultTrialConfig.update_forward_refs()
+SubscriptionScheduledUpdateData.update_forward_refs()
+SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 SubscriptionFutureUpdateData.update_forward_refs()
 SubscriptionFutureUpdateDataTargetPackage.update_forward_refs()
 SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 TotalPriceFragment.update_forward_refs()
 TotalPriceFragmentSubTotal.update_forward_refs()
 TotalPriceFragmentTotal.update_forward_refs()
-SubscriptionScheduledUpdateData.update_forward_refs()
-SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 SubscriptionFragment.update_forward_refs()
 SubscriptionFragmentResource.update_forward_refs()
 SubscriptionFragmentExperimentInfo.update_forward_refs()
 SubscriptionFragmentPrices.update_forward_refs()
 SubscriptionFragmentPricesPrice.update_forward_refs()
 SubscriptionFragmentTotalPrice.update_forward_refs()
 SubscriptionFragmentPlan.update_forward_refs()
@@ -1509,19 +1509,19 @@
 UsageUpdatedFragment.update_forward_refs()
 EntitlementUsageUpdated.update_forward_refs()
 EntitlementUsageUpdatedUsage.update_forward_refs()
 EntitlementUsageUpdatedEntitlement.update_forward_refs()
 EntitlementsUpdatedPayload.update_forward_refs()
 EntitlementsUpdatedPayloadEntitlements.update_forward_refs()
 LayoutConfigurationFragment.update_forward_refs()
+MockPaywallPackageEntitlementFragment.update_forward_refs()
+MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallPriceFragment.update_forward_refs()
 MockPaywallPriceFragmentPrice.update_forward_refs()
 MockPaywallPriceFragmentFeature.update_forward_refs()
-MockPaywallPackageEntitlementFragment.update_forward_refs()
-MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallAddonFragment.update_forward_refs()
 MockPaywallAddonFragmentEntitlements.update_forward_refs()
 MockPaywallAddonFragmentPrices.update_forward_refs()
 MockPaywallPlanFragment.update_forward_refs()
 MockPaywallPlanFragmentProduct.update_forward_refs()
 MockPaywallPlanFragmentBasePlan.update_forward_refs()
 MockPaywallPlanFragmentEntitlements.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.523.0/stigg/generated/get_active_subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.523.0/stigg/generated/get_coupons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.523.0/stigg/generated/get_customer_by_id.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.523.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.523.0/stigg/generated/get_mock_paywall.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.523.0/stigg/generated/get_sdk_configuration.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.523.0/stigg/generated/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.523.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.523.0/stigg/generated/provision_customer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.523.0/stigg/generated/provision_subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.523.0/stigg/generated/report_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.522.0/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.523.0/stigg/generated/update_subscription.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 12:59
+# Generated by ariadne-codegen on 2023-08-05 17:44
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.522.0/PKG-INFO` & `stigg_api_client_v2-0.523.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.522.0
+Version: 0.523.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

