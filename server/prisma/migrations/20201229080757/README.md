# Migration `20201229080757`

This migration has been generated by JunIshino at 12/29/2020, 5:07:57 PM.
You can check out the [state of the schema](./schema.prisma) after the migration.

## Database Steps

```sql

```

## Changes

```diff
diff --git schema.prisma schema.prisma
migration ..20201229080757
--- datamodel.dml
+++ datamodel.dml
@@ -1,0 +1,14 @@
+datasource db {
+  provider = "postgresql"
+  url = "***"
+}
+
+generator client {
+  provider = "prisma-client-js"
+}
+
+model Task {
+  id    Int     @id @default(autoincrement())
+  label String
+  done  Boolean @default(false)
+}
```


