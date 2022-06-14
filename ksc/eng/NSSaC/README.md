# Nurion System Specifications and Configuration

****
<div id="contents" class="content" style="margin-left: 320px;">




<h1 id="jcsTitle" class="title-01">Nurion System Specifications and Configuration</h1>
<div class="clear-float"></div>
<div class="space-div"></div>
<div id="jcsContents" class="contnet">
	<h1><strong>A. Overview</strong></h1><a class="tit_anchor" id="docout-0"></a>
<p>Nurion, which is KISTI's 5th supercomputer, is a Linux-based massively parallel cluster system that exhibits a total theoretical operation performance (Rpeak) of 25.7 PFlops (approximately 70 times that of the 4th supercomputer, Tachyon2).</p>
<p>&nbsp;</p>
<p>Nurion consists of 8,305 manycore CPUs (consisting of 68 cores) that have a performance of 3 TFlops (1/100 of the overall performance of Tachyon2, the 4th supercomputer) per socket (CPU) and is consequently a cluster-based supercomputing system in which tens of thousands of cores can be utilized simultaneously. It is also equipped with high-performance interconnect, mass storage, and a burst buffer. A burst buffer can efficiently process the massive I/O requests that occur instantly in application programs.</p>
<p>&nbsp;</p>
<p>Nurion aims to help improve national R&amp;D competence based on its large-scale computational capability and to solve complicated problems such as weather prediction or new material development as well as expensive and dangerous experiments involving aviation or new drug development. In an effort to solve different problems related to scientific technology, difficult problems are being discovered across a variety of fields even in the planning phase.</p>
<p>&nbsp;</p>
<p>Various types of software are equipped and consistently upgraded in Nurion to support R&amp;D efforts, while high-performance hardware are linked to maintain the highest productivity. Furthermore, Nurion intends to become essential infrastructure for implementing an intelligent information society and advancing national scientific technology through user support such as through optimization, parallelization, and large project discovery for solving significant challenges.</p>
<p>&nbsp;</p>
<p><img style="display: block; margin-left: auto; margin-right: auto;" src="../../../../file/image/?path=sos/jcs/2021/11/&amp;name=hZUlzJMzieep1fc.png"></p>
<p style="text-align: center;">&nbsp;</p>
<p style="text-align: center;">[Block diagram of Nurion]</p>
<p>&nbsp;</p>
<table class="common-table-03 txt-ac" border="0" cellspacing="0" cellpadding="0"><colgroup><col style="width: 30%;"></colgroup><colgroup><col style="width: 30%;"></colgroup><colgroup><col style="width: 20%;"></colgroup><colgroup><col style="width: 20%;"></colgroup>
<thead>
<tr>
<th style="width: 415px;" colspan="2">Category</th>
<th style="width: 124px;">KNL Computing node</th>
<th style="width: 124px;">CPU-only node</th>
</tr>
<!-- <td colspan="2" width="60%">
<p><strong>Category</strong></p>
</td>
<td width="18%">
<p><strong>KNL Computing node</strong></p>
</td>
<td width="21%">
<p><strong>CPU-only node</strong></p>
</td> --></thead>
<tbody>
<tr>
<td colspan="2" width="60%">
<p>Manufacturer and model</p>
</td>
<td colspan="2" width="39%">
<p>Cray CS500</p>
</td>
</tr>
<tr>
<td colspan="2" width="60%">
<p>No. of nodes</p>
</td>
<td width="18%">
<p>8,305</p>
</td>
<td width="21%">
<p>132</p>
</td>
</tr>
<tr>
<td colspan="2" width="60%">
<p>Theoretical peak performance (Rpeak)</p>
</td>
<td width="18%">
<p>25.3 PFlops</p>
</td>
<td width="21%">
<p>0.4 PFlops</p>
</td>
</tr>
<tr>
<td rowspan="5" width="28%">
<p>Processor</p>
</td>
<td width="31%">
<p>Model</p>
</td>
<td width="18%">
<p>Intel Xeon Phi 7250(KNL)</p>
</td>
<td width="21%">
<p>Intel Xeon 6148 (Skylake)</p>
</td>
</tr>
<tr>
<td width="31%">
<p>Theoretical performance per CPU</p>
</td>
<td width="18%">
<p>3.0464 TFLOPS</p>
</td>
<td width="21%">
<p>1.536 TFLOPS</p>
</td>
</tr>
<tr>
<td width="31%">
<p>No. of cores per CPU</p>
</td>
<td width="18%">
<p>68</p>
</td>
<td width="21%">
<p>20</p>
</td>
</tr>
<tr>
<td width="31%">
<p>No. of CPUs per node</p>
</td>
<td width="18%">
<p>1</p>
</td>
<td width="21%">
<p>2</p>
</td>
</tr>
<tr>
<td width="31%">
<p>On-package Memory</p>
</td>
<td width="18%">
<p>16GB, 490GB/s</p>
</td>
<td width="21%">
<p>-</p>
</td>
</tr>
<tr>
<td rowspan="5" width="28%">
<p>Main memory</p>
</td>
<td width="31%">
<p>Model</p>
</td>
<td width="18%">
<p>16GB DDR4-2400</p>
</td>
<td width="21%">
<p>16GB DDR4-2666</p>
</td>
</tr>
<tr>
<td width="31%">
<p>Configuration</p>
</td>
<td width="18%">
<p>16GB x6, 6Ch per CPU</p>
</td>
<td width="21%">
<p>16GB x12, 6Ch per CPU</p>
</td>
</tr>
<tr>
<td width="31%">
<p>Memory per node (GB)</p>
</td>
<td width="18%">
<p>96GB</p>
</td>
<td width="21%">
<p>192GB</p>
</td>
</tr>
<tr>
<td width="31%">
<p>Bandwidth per CPU</p>
</td>
<td width="18%">
<p>115.2GB/s</p>
</td>
<td width="21%">
<p>128GB/s</p>
</td>
</tr>
<tr>
<td width="31%">
<p>Total size</p>
</td>
<td width="18%">
<p>778.6TB</p>
</td>
<td width="21%">
<p>24.8TB</p>
</td>
</tr>
<tr>
<td rowspan="4" width="28%">
<p>High-performance interconnect</p>
</td>
<td width="31%">
<p>Topology</p>
</td>
<td colspan="2" width="39%">
<p>Fat Tree</p>
</td>
</tr>
<tr>
<td width="31%">
<p>Blocking Ratio</p>
</td>
<td colspan="2" width="39%">
<p>50% Blocking</p>
</td>
</tr>
<tr>
<td width="31%">
<p>Switches configuration</p>
</td>
<td colspan="2" width="39%">
<p>278x 48-port OPA edge switches<br> 8x 768-port OPA core switches</p>
</td>
</tr>
<tr>
<td width="31%">
<p>Bandwidth per port</p>
</td>
<td colspan="2" width="39%">
<p>100Gbps</p>
</td>
</tr>
<tr>
<td rowspan="4" width="28%">
<p>High-performance filesystem (burst buffer)</p>
</td>
<td width="31%">
<p>No. of servers</p>
</td>
<td colspan="2" width="39%">
<p>DDN IME240 Server 48ea</p>
</td>
</tr>
<tr>
<td width="31%">
<p>Disk per server</p>
</td>
<td colspan="2" width="39%">
<p>16x 1.2TB NVMe SSD, 2x 0.45TB NVMe SSD</p>
</td>
</tr>
<tr>
<td width="31%">
<p>Total available capacity</p>
</td>
<td colspan="2" width="39%">
<p>0.8PB</p>
</td>
</tr>
<tr>
<td width="31%">
<p>Bandwidth</p>
</td>
<td colspan="2" width="39%">
<p>20GB/sec per server, 0.8TB/s total</p>
</td>
</tr>
<tr>
<td rowspan="4" width="28%">
<p>Parallel filesystem</p>
</td>
<td width="31%">
<p>File system</p>
</td>
<td colspan="2" width="39%">
<p>Lustre 2.7.21.3</p>
</td>
</tr>
<tr>
<td width="31%">
<p>Total available capacity</p>
</td>
<td colspan="2" width="39%">
<p>/scratch: 21PB, /home: 0.76PB, /apps: 0.5PB</p>
</td>
</tr>
<tr>
<td width="31%">
<p>Bandwidth</p>
</td>
<td colspan="2" width="39%">
<p>0.3TB/s</p>
</td>
</tr>
<tr>
<td width="31%">
<p>RAID configuration</p>
</td>
<td colspan="2" width="39%">
<p>RAID6(8D+2P)</p>
</td>
</tr>
</tbody>
</table>
<p style="text-align: center;">&nbsp;</p>
<p style="text-align: center;">[Nurion system specifications and configuration]</p>
<p>&nbsp;</p>
<h1>B. Computing Node</h1><a class="tit_anchor" id="docout-1"></a>
<p>There are a total of 8,437 computing nodes in the Nurion system, among which 8,305 are equipped with the manycore-based Intel Xeon Phi 7250 processor, whereas 132 of them are equipped with the Intel Xeon Gold 6148 processor.</p>
<p>&nbsp;</p>
<h3>KNL (manycore) node</h3>
<p>The Intel Xeon Phi 7250 processor (code name: Knights Landing) equipped in the KNL node is operated by 68 cores (hyper threading off) at a fundamental frequency of 1.4 GHz. The L2 cache memory is 34 MB, and the Multi-Channel DRAM (MCDRAM), which is an on-package memory, is 16 GB (490 GB/s bandwidth). The memory per node is 96 GB, consisting of six channels of 16 GB DDR4-2400 memory. The 2U-size enclosure is equipped with four computing nodes, in which the 42U standard rack consists of 72 computing nodes.</p>
<p><img style="display: block; margin-left: auto; margin-right: auto;" src="../../../../file/image/?path=sos/jcs/2021/11/&amp;name=M9lQKV9UwdVVho0.png"></p>
<p style="text-align: center;">[Block diagram of KNL-based computing node]</p>
<p style="text-align: center;">&nbsp;</p>
<p><img style="display: block; margin-left: auto; margin-right: auto;" src="../../../../file/image/?path=sos/jcs/2021/11/&amp;name=8eTQgXRi3rFKRQO.png"></p>
<p style="text-align: center;">[KNL-based computing node]</p>
<p>&nbsp;</p>
<h3>SKL (CPU-only) node</h3>
<p>The SKL (CPU-only) node is equipped with two Intel Xeon Gold 6148 processors (code name: Skylake). The fundamental frequency is 2.4 GHz, and there are 20 CPU cores (hyperthreading off). The L3 cache memory is 27.5 MB, and the memory per CPU is 96 GB (192 GB per node) with six channels of 16 GB DDR4-2666 memory. The 2U-size enclosure is equipped with four computing nodes.</p>
<p><img style="display: block; margin-left: auto; margin-right: auto;" src="../../../../file/image/?path=sos/jcs/2021/11/&amp;name=NwiAvTQB3n1mbjQ.png"></p>
<p style="text-align: center;">[Block diagram of SKL-based CPU-only node]</p>
<p style="text-align: center;">&nbsp;</p>
<p><img style="display: block; margin-left: auto; margin-right: auto;" src="../../../../file/image/?path=sos/jcs/2021/11/&amp;name=h3jV5a33UZiVL0I.png"></p>
<p style="text-align: center;">[SKL-based CPU-only node]</p>
<p style="text-align: center;">&nbsp;</p>
<h1>C. Interconnect Network</h1><a class="tit_anchor" id="docout-2"></a>
<p>It uses Intel’s Omni-Path Architecture (OPA) as the computing network between nodes and the interconnect network for file I/O communications. In a fat-tree topology using 100 Gbps OPA, the network is configured with 50% blocking between the computing nodes and non-blocking between storage units. The computing nodes and storage units are connected to 277 48-port OPA Edge switches, and all Edge switches are connected to eight 768-port OPA Director switches.</p>
<p><img style="display: block; margin-left: auto; margin-right: auto;" src="../../../../file/image/?path=sos/jcs/2021/11/&amp;name=89LSApl4oE0nAN0.png"></p>
<p style="text-align: center;">[Block diagram of interconnect network]</p>
<p>&nbsp;</p>
<h1>D. Storage</h1><a class="tit_anchor" id="docout-3"></a>
<h3>Parallel filesystem and burst buffer configuration</h3>
<p>Nurion provides a parallel filesystem and burst buffer configuration for I/O processing and data storage. Three Lustre filesystems, namely scratch (/scratch 21PB), home (/home01, 760TB), and application (/app, 507TB), are provided for the parallel filesystem.</p>
<p>&nbsp;</p>
<p>Each filesystem consists of an SFA7700X storage-based metadata server (MDS) and an ES14KX storage-based object storage server (OSS). The burst buffer is an NVMe based I/O cache that acts between computing nodes and the parallel filesystem and provides approximately 844 TB capacity. The Lustre filesystem provides I/O services by being mounted on the computing node, login node, and archiving server (data mover).</p>
<p><img style="display: block; margin-left: auto; margin-right: auto;" src="../../../../file/image/?path=sos/jcs/2021/11/&amp;name=sOdKlUWMwnbB9lP.png"></p>
<p style="text-align: center;">[Configuration of parallel filesystem and overall burst buffer rack]</p>
<p style="text-align: center;">&nbsp;</p>
<p><img style="display: block; margin-left: auto; margin-right: auto;" src="../../../../file/image/?path=sos/jcs/2021/11/&amp;name=UikUtB7HWx9PSti.png"></p>
<p style="text-align: center;">[PFS server configuration]</p>
<p>&nbsp;</p>
<h3>Burst Buffer</h3>
<p>- Overview</p>
<p>Burst buffer (hereinafter, “BB”) is a cache layer between the computing node and storage (/scratch) for I/O acceleration; it was newly introduced in the 5th supercomputer to maximize the performance of the parallel I/O and supplement the low performance for small or random I/O in the parallel filesystem. It aims to enhance the performance of user applications with high I/O dependency and supports all queues using KNL nodes.</p>
<p>&nbsp;</p>
<p style="text-align: center;">&nbsp;&nbsp;&nbsp;&nbsp;<img src="../../../../file/image/?path=sos/jcs/2020/02/&amp;name=6n7FDTWgDLwFPaD.png">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp;<img src="../../../../file/image/?path=sos/jcs/2020/02/&amp;name=ijCBgRkhSskY4Fv.png"></p>
<p style="text-align: center;">&nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Burst Buffer role]&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; [Burst Buffer server configuration]</p>
<p>&nbsp;</p>
<p>- System configuration</p>
<p>The IME240 solution of DDN was applied for the BB configuration; the [Burst buffer server configuration] figure above shows the detailed configuration of the BB.</p>
<p>&nbsp;</p>
<table class="common-table-03 txt-ac" border="0" cellspacing="0" cellpadding="0"><colgroup><col style="width: 30%;"></colgroup><colgroup><col style="width: 70%;"></colgroup>
<tbody>
<tr>
<th>System</th>
<td style="text-align: center;">DDN IME240, Infinite Memory Engine Appliance</td>
</tr>
<tr>
<th>Software version</th>
<td style="text-align: center;">CentOS 7.4, IME 1.3</td>
</tr>
<tr>
<th>Max. I/O performance</th>
<td style="text-align: center;">20 GB/s</td>
</tr>
<tr>
<th>Network interface</th>
<td style="text-align: center;">2 x OPA</td>
</tr>
<tr>
<th>SSD type</th>
<td style="text-align: center;">1.2TB, NVMe drive</td>
</tr>
<tr>
<th>SDD quantity</th>
<td style="text-align: center;">16ea(1.2TB NVMe) + 1ea(450GB SSD)</td>
</tr>
<tr>
<th>Capacity (RAW)</th>
<td style="text-align: center;">19.2TB</td>
</tr>
</tbody>
</table>
<p style="text-align: center;">&nbsp;</p>
<p style="text-align: center;">[IME single node configuration]</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<table class="common-table-03 txt-ac" border="0" cellspacing="0" cellpadding="0"><colgroup><col style="width: 30%;"></colgroup><colgroup><col style="width: 70%;"></colgroup>
<tbody>
<tr>
<th>Total no. of systems</th>
<td>IME240 x 48</td>
</tr>
<tr>
<th>Total capacity (RAW)</th>
<td>979.2 TB</td>
</tr>
<tr>
<th>Total capacity (when parity is applied))</th>
<td>816 TB (EC*, 10+2)</td>
</tr>
<tr>
<th>Max. I/O performance</th>
<td>800 GB/s</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p style="text-align: center;">[Overall configuration of burst buffer]</p>
<p>&nbsp;</p>
<p>*EC : Erasure Coding (settings may change)</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
</div>
