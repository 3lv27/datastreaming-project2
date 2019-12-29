# SF Crime Project

### 1. How did changing values on the SparkSession property parameters affect the throughput and latency of the data?

We can see the impact of these values encreasing or decreasing  `processedRowsPerSecond` and `inputRowsPerSecond`


### 2. What were the 2-3 most efficient SparkSession property key/value pairs? Through testing multiple variations on values, how can you tell these were the most optimal?

To ensure the values I was playing around were the most optimal I used the value of `processedRowsPerSecond` obtaining `341.8551515158866`

The params I found more relevant:

```
spark.sql.shuffle.partitions                
spark.streaming.kafka.maxRatePerPartition   
```
