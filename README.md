# siddhi-runner-beam

**siddhi-runner-beam** is a java library that executes a pipeline from <a target="_blank" href="https://beam.apache.org/">Apache Beam</a> in <a target="_blank" href="https://wso2.github.io/siddhi">Siddhi</a>.

## How to Use

* Add the runner library as a maven dependancy along with other Beam dependancies.

```
     <dependency>
        <groupId>org.wso2.siddhi.runner.beam</groupId>
        <artifactId>siddhi-runner-beam</artifactId>
        <version>x.x.x</version>
     </dependency>
```

* Set the runner of the pipeline as _SiddhiRunner_.

```
     //SiddhiPipelineOptions is defined
     SiddhiPipelineOptions options = PipelineOptionsFactory.as(SiddhiPipelineOptions.class);
     options.setRunner(SiddhiRunner.class);
```

## Features

Below is the list of transforms that are currently supported.

* ParDo
* GroupByKey
* FixedWindow
* Flatten
* Partition
* TextIO


 