diff --git a/ldm/util.py b/ldm/util.py
index 8c09ca1..681ffcf 100644
--- a/ldm/util.py
+++ b/ldm/util.py
@@ -76,7 +76,7 @@ def instantiate_from_config(config):
         elif config == "__is_unconditional__":
             return None
         raise KeyError("Expected key `target` to instantiate.")
-    return get_obj_from_str(config["target"])(**config.get("params", dict()))
+    return get_obj_from_str(config["target"])(**config.get("params", dict())).cuda()
 
 
 def get_obj_from_str(string, reload=False):
