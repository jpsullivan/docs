---
title: Module efs
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->

<a href="../index.html">@pulumi/awsx</a> &gt; efs

<div class="toggleVisible" markdown="1">
<div class="collapsed" markdown="1">
<h2 class="pdoc-module-header toggleButton" title="Click to show Index">Index ▹</h2>
</div>
<div class="expanded" markdown="1">
<h2 class="pdoc-module-header toggleButton" title="Click to hide Index">Index ▾</h2>
<div class="pdoc-module-contents" markdown="1">
* <a href="#burstCreditBalance">function burstCreditBalance</a>
* <a href="#clientConnections">function clientConnections</a>
* <a href="#dataReadIOBytes">function dataReadIOBytes</a>
* <a href="#dataWriteIOBytes">function dataWriteIOBytes</a>
* <a href="#metadataIOBytes">function metadataIOBytes</a>
* <a href="#metric">function metric</a>
* <a href="#percentIOLimit">function percentIOLimit</a>
* <a href="#permittedThroughput">function permittedThroughput</a>
* <a href="#totalIOBytes">function totalIOBytes</a>
* <a href="#EfsMetricChange">interface EfsMetricChange</a>
* <a href="#EfsMetricName">type EfsMetricName</a>

<a href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/efs/metrics.ts">efs/metrics.ts</a> 
</div>
</div>
</div>


<h2 class="pdoc-module-header" id="burstCreditBalance">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/efs/metrics.ts#L79">function <b>burstCreditBalance</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">

<pre class="highlight"><span class='kd'></span>burstCreditBalance(change?: <a href='#EfsMetricChange'>EfsMetricChange</a>): <a href='#Metric'>Metric</a></pre>


The number of burst credits that a file system has.

Burst credits allow a file system to burst to throughput levels above a file system’s
baseline level for periods of time. For more information, see Throughput scaling in Amazon
EFS.

The Minimum statistic is the smallest burst credit balance for any minute during the period.
The Maximum statistic is the largest burst credit balance for any minute during the period.
The Average statistic is the average burst credit balance during the period.

Units: Bytes

Valid statistics: Minimum, Maximum, Average

</div>
<h2 class="pdoc-module-header" id="clientConnections">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/efs/metrics.ts#L94">function <b>clientConnections</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">

<pre class="highlight"><span class='kd'></span>clientConnections(change?: <a href='#EfsMetricChange'>EfsMetricChange</a>): <a href='#Metric'>Metric</a></pre>


The number of client connections to a file system. When using a standard client, there is one
connection per mounted Amazon EC2 instance.

Note: To calculate the average ClientConnections for periods greater than one minute, divide
the Sum statistic by the number of minutes in the period.

Units: Count of client connections

Valid statistics: Sum

</div>
<h2 class="pdoc-module-header" id="dataReadIOBytes">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/efs/metrics.ts#L113">function <b>dataReadIOBytes</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">

<pre class="highlight"><span class='kd'></span>dataReadIOBytes(change?: <a href='#EfsMetricChange'>EfsMetricChange</a>): <a href='#Metric'>Metric</a></pre>


The number of bytes for each file system read operation.

The Sum statistic is the total number of bytes associated with read operations. The Minimum
statistic is the size of the smallest read operation during the period. The Maximum statistic
is the size of the largest read operation during the period. The Average statistic is the
average size of read operations during the period. The SampleCount statistic provides a count
of read operations.

Units:
* Bytes for Minimum, Maximum, Average, and Sum.
* Count for SampleCount.

Valid statistics: Minimum, Maximum, Average, Sum, SampleCount

</div>
<h2 class="pdoc-module-header" id="dataWriteIOBytes">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/efs/metrics.ts#L132">function <b>dataWriteIOBytes</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">

<pre class="highlight"><span class='kd'></span>dataWriteIOBytes(change?: <a href='#EfsMetricChange'>EfsMetricChange</a>): <a href='#Metric'>Metric</a></pre>


The number of bytes for each file write operation.

The Sum statistic is the total number of bytes associated with write operations. The Minimum
statistic is the size of the smallest write operation during the period. The Maximum
statistic is the size of the largest write operation during the period. The Average statistic
is the average size of write operations during the period. The SampleCount statistic provides
a count of write operations.

Units:
* Bytes for Minimum, Maximum, Average, and Sum.
* Count for SampleCount.

Valid statistics: Minimum, Maximum, Average, Sum, SampleCount

</div>
<h2 class="pdoc-module-header" id="metadataIOBytes">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/efs/metrics.ts#L151">function <b>metadataIOBytes</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">

<pre class="highlight"><span class='kd'></span>metadataIOBytes(change?: <a href='#EfsMetricChange'>EfsMetricChange</a>): <a href='#Metric'>Metric</a></pre>


The number of bytes for each metadata operation.

The Sum statistic is the total number of bytes associated with metadata operations. The
Minimum statistic is the size of the smallest metadata operation during the period. The
Maximum statistic is the size of the largest metadata operation during the period. The
Average statistic is the size of the average metadata operation during the period. The
SampleCount statistic provides a count of metadata operations.

Units:
* Bytes for Minimum, Maximum, Average, and Sum.
* Count for SampleCount.

Valid statistics: Minimum, Maximum, Average, Sum, SampleCount

</div>
<h2 class="pdoc-module-header" id="metric">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/efs/metrics.ts#L51">function <b>metric</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">

<pre class="highlight"><span class='kd'></span>metric(metricName: <a href='#EfsMetricName'>EfsMetricName</a>, change: <a href='#EfsMetricChange'>EfsMetricChange</a>): <a href='#Metric'>Metric</a></pre>


Creates an AWS/EFS metric with the requested [metricName]. See
https://docs.aws.amazon.com/efs/latest/ug/monitoring-cloudwatch.html for list of all
metric-names.

Note, individual metrics can easily be obtained without supplying the name using the other
[metricXXX] functions.

You can monitor file systems using Amazon CloudWatch, which collects and processes raw data from
Amazon EFS into readable, near real-time metrics. These statistics are recorded for a period of
15 months, so that you can access historical information and gain a better perspective on how
your web application or service is performing. By default, Amazon EFS metric data is
automatically sent to CloudWatch at 1-minute periods.

Amazon EFS metrics use the EFS namespace and provides metrics for a single dimension,
"FileSystemId". A file system's ID can be found in the Amazon EFS management console, and it
takes the form of fs-XXXXXXXX.

</div>
<h2 class="pdoc-module-header" id="percentIOLimit">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/efs/metrics.ts#L165">function <b>percentIOLimit</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">

<pre class="highlight"><span class='kd'></span>percentIOLimit(change?: <a href='#EfsMetricChange'>EfsMetricChange</a>): <a href='#Metric'>Metric</a></pre>


Shows how close a file system is to reaching the I/O limit of the General Purpose performance
mode. If this metric is at 100% more often than not, consider moving your application to a
file system using the Max I/O performance mode.

Note: This metric is only submitted for file systems using the General Purpose performance
mode.

Units: Percent

</div>
<h2 class="pdoc-module-header" id="permittedThroughput">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/efs/metrics.ts#L185">function <b>permittedThroughput</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">

<pre class="highlight"><span class='kd'></span>permittedThroughput(change?: <a href='#EfsMetricChange'>EfsMetricChange</a>): <a href='#Metric'>Metric</a></pre>


The maximum amount of throughput a file system is allowed. For file systems in the
Provisioned Throughput mode, if the amount of storage allows your file system to drive a
higher amount of throughput than you provisioned, this metric will reflect the higher
throughput instead of the provisioned amount. For file systems in the Bursting Throughput
mode, this value is a function of the file system size and BurstCreditBalance. For more
information, see Amazon EFS Performance.

The Minimum statistic is the smallest throughput permitted for any minute during the period.
The Maximum statistic is the highest throughput permitted for any minute during the period.
The Average statistic is the average throughput permitted during the period.

Units: Bytes per second

Valid statistics: Minimum, Maximum, Average

</div>
<h2 class="pdoc-module-header" id="totalIOBytes">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/efs/metrics.ts#L209">function <b>totalIOBytes</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">

<pre class="highlight"><span class='kd'></span>totalIOBytes(change?: <a href='#EfsMetricChange'>EfsMetricChange</a>): <a href='#Metric'>Metric</a></pre>


The number of bytes for each file system operation, including data read, data write, and
metadata operations.

The Sum statistic is the total number of bytes associated with all file system operations.
The Minimum statistic is the size of the smallest operation during the period. The Maximum
statistic is the size of the largest operation during the period. The Average statistic is
the average size of an operation during the period. The SampleCount statistic provides a
count of all operations.

Note: To calculate the average operations per second for a period, divide the SampleCount
statistic by the number of seconds in the period. To calculate the average throughput (Bytes
per second) for a period, divide the Sum statistic by the number of seconds in the period.

Units:
Bytes for Minimum, Maximum, Average, and Sum statistics.
Count for SampleCount.

Valid statistics: Minimum, Maximum, Average, Sum, SampleCount

</div>
<h2 class="pdoc-module-header" id="EfsMetricChange">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/efs/metrics.ts#L26">interface <b>EfsMetricChange</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">
<pre class="highlight"><span class='kd'>extends</span> <a href='#MetricChange'>MetricChange</a></pre>
<h3 class="pdoc-member-header" id="EfsMetricChange-color">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/cloudwatch/metric.ts#L439">property <b>color</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>color?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>

The six-digit HTML hex color code to be used for this metric.

Only used if this metric is displayed in a [Dashboard] with a [MetricWidget].

</div>
<h3 class="pdoc-member-header" id="EfsMetricChange-dimensions">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/cloudwatch/metric.ts#L408">property <b>dimensions</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>dimensions?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;Record&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>&gt;&gt;;</pre>

The new dimension for this metric.  If this object is missing this property, then no change
will be made.  However, if the property is there by set to [undefined] then the value will be
cleared.

</div>
<h3 class="pdoc-member-header" id="EfsMetricChange-extendedStatistic">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/cloudwatch/metric.ts#L426">property <b>extendedStatistic</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>extendedStatistic?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number'>number</a></span>&gt;;</pre>

The new percentile statistic for the metric associated with the alarm.  If this object is
missing this property, then no change will be made.  However, if the property is there by set
to [undefined] then the value will be set to the default.

</div>
<h3 class="pdoc-member-header" id="EfsMetricChange-fileSystem">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/efs/metrics.ts#L30">property <b>fileSystem</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>fileSystem?: aws.efs.FileSystem;</pre>

Filters down events to the specified [FileSystem].

</div>
<h3 class="pdoc-member-header" id="EfsMetricChange-label">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/cloudwatch/metric.ts#L448">property <b>label</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>label?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>

The label to display for this metric in the graph legend. If this is not specified, the
metric is given an autogenerated label that distinguishes it from the other metrics in the
widget.

Only used if this metric is displayed in a [Dashboard] with a [MetricWidget].

</div>
<h3 class="pdoc-member-header" id="EfsMetricChange-period">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/cloudwatch/metric.ts#L414">property <b>period</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>period?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number'>number</a></span>&gt;;</pre>

The new period in seconds over which the specified `stat` is applied.  If this object is
missing this property, then no change will be made.  However, if the property is there by set
to [undefined] then the value will be set to the default (300s).

</div>
<h3 class="pdoc-member-header" id="EfsMetricChange-statistic">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/cloudwatch/metric.ts#L420">property <b>statistic</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>statistic?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='#MetricStatistic'>MetricStatistic</a>&gt;;</pre>

The new statistic to apply to the alarm's associated metric.  If this object is missing this
property, then no change will be made.  However, if the property is there by set to
[undefined] then the value will be set to the default.

</div>
<h3 class="pdoc-member-header" id="EfsMetricChange-unit">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/cloudwatch/metric.ts#L432">property <b>unit</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>unit?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='#MetricUnit'>MetricUnit</a>&gt;;</pre>

The new unit for this metric.   If this object is missing this property, then no change will
be made.  However, if the property is there by set to [undefined] then the value will be set
to the default.

</div>
<h3 class="pdoc-member-header" id="EfsMetricChange-visible">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/cloudwatch/metric.ts#L456">property <b>visible</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>visible?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span>&gt;;</pre>

Set this to true to have the metric appear in the graph, or false to have it be hidden. The
default is true.

Only used if this metric is displayed in a [Dashboard] with a [MetricWidget].

</div>
<h3 class="pdoc-member-header" id="EfsMetricChange-yAxis">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/cloudwatch/metric.ts#L463">property <b>yAxis</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>yAxis?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='s2'>"left"</span> | <span class='s2'>"right"</span>&gt;;</pre>

Where on the graph to display the y-axis for this metric. The default is left.

Only used if this metric is displayed in a [Dashboard] with a [MetricWidget].

</div>
</div>
<h2 class="pdoc-module-header" id="EfsMetricName">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-awsx/blob/master/nodejs/awsx/efs/metrics.ts#L21">type <b>EfsMetricName</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">
<pre class="highlight"><span class='kd'>type</span> EfsMetricName = <span class='s2'>"BurstCreditBalance"</span> | <span class='s2'>"ClientConnections"</span> | <span class='s2'>"DataReadIOBytes"</span> | <span class='s2'>"DataWriteIOBytes"</span> | <span class='s2'>"MetadataIOBytes"</span> | <span class='s2'>"PercentIOLimit"</span> | <span class='s2'>"PermittedThroughput"</span> | <span class='s2'>"TotalIOBytes"</span>;</pre>
</div>