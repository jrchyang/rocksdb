For Leveled Compaction users, `CompactRange()` will now always try to compact to the last non-empty level. (#11468)
For Leveled Compaction users, `CompactRange()` with `bottommost_level_compaction = BottommostLevelCompaction::kIfHaveCompactionFilter` will behave similar to `kForceOptimized` in that it will skip files created during this manual compaction when compacting files in the bottommost level. (#11468)