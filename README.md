# ece4016-assignment-2--adaptive-bitrate-streaming-solved
**TO GET THIS SOLUTION VISIT:** [ECE4016 Assignment 2- Adaptive Bitrate Streaming Solved](https://www.ankitcodinghub.com/product/ece4016-adaptive-bitrate-streaming-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;116094&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;ECE4016 Assignment 2- Adaptive Bitrate Streaming Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
This project aims to learn high-level thought and implement a demo of adaptive bitrate (ABR) algorithms for video streaming. We provide the video simulator, which will simulate video download and playback and continuously execute the user-written algorithm for bitrate decisions. We will first introduce the whole picture of video bitrate adaptation, then illustrate the task you need to finish and show a paper list of ABR algorithms. The algorithm you write will be tested over various simulated network environments and ultimately be given a final quality of experience(QoE) score.

0x01 Overview – What is adaptive bitrate streaming?

Adaptive bitrate streaming is a method for improving streaming over HTTP networks. The term

“bitrate” refers to how quickly data travels across a network and is often used to describe an

Internet connection’s speed. A high-speed connection is a high-bitrate connection. Streaming — or the process that makes watching videos online possible — consists of transmitting video files hosted on a remote server to a client. In streaming, videos are segmented into smaller clips so viewers do not need to wait for an entire video to load before they can begin watching it.

First, multiple versions of video files are created and encoded to fit a variety of network conditions. Then, based on factors like bandwidth and device type, the video player selects the highest-quality file that the device can play with the smallest amount of buffering possible. This allows playback to be as smooth as possible for end users worldwide, regardless of device or Internet speed.

0x02 ABR Architecture – How does adaptive bitrate streaming work?

ABR starts with your raw data, and it is prepped before streaming. Video is transcoded and segmented into chunks. After this, the process is up to the playback device, which requests these chunks of data according to what it can handle given the available bandwidth. Let’s look at these steps in more detail and some factors that might affect how they work.

Video Encoding and Transcoding

Encoding is the process by which raw video data is compressed and prepared for transport to a playback device. Transcoding is the process by which already compressed data is decompressed and decoded to alter it, often resulting in multiple versions of the original data. These changes are typical as follows:

Resizing the video frame rate – or resolution – to accommodate different screens.

Changing the bitrate of the decompressed file to accommodate different connection speeds. This can include changing the frame rate or the resolution.

Transrating is critical to adaptive bitrate streaming. After all, a playback device can’t access data at a specific bitrate or resolution if it doesn’t exist in that form.

Video Segmenting

You now have a collection of various sizes and resolutions for your video data that a playback device can access. But what if the playback device chooses incorrectly and the bitrate of the selected file is not ideal for the available bandwidth?

This is where segmenting comes in. Also known as chunked encoding, or chunking, this is the process by which streaming data is separated into a series of non-overlapping segments before being sent to the playback device. Each chunk typically ranges in length from 2 to 10 seconds. By breaking up the data this way, it’s possible to adjust the size of data sent to a playback device mid-stream.

Initial Startup

Now that the data is fully prepared, the viewer’s playback device takes the wheel. Before streaming begins, the playback device downloads a manifest that describes all the available chunks and bitrates. This is a menu from which the playback device can start streaming. Typically, a playback device will take it slow, selecting a bitrate it knows it can handle before adjusting.

Video Playback

After each segment, the playback device recalibrates and requests the next segment based on the new information. For example, the first segment was likely a much lower bitrate than necessary. The device will then request a higher bitrate for the next segment. If the bandwidth lessens or the device struggles to play a segment, it will adjust downward when requesting the next one.

0x03 Tasks

We provide several different tasks. You need to choose and finish one of them.

Task-1: (Complete it alone)

Read a paper of ABR algorithm, and implement the corresponding ABR algorithm according to the paper. Submit a 2 pages pdf report, including Algorithm Analysis , Implementation , and Evaluation. Grading:

Program implementation: 70%. Report score: 30%.

Task-2: (A group up to 3 people)

Design an ABR algorithm by yourself, write the code, and submit a 4 pages pdf report, including

Algorithm Design, Implementation, and Evaluation. Please describe the mathematical

model / algorithms / neural network structure / dynamic programming transition function or any other methods you use in your algorithm. You can use pictures, pseudocode, and formulas to illustrate them.

Grading:

Program implementation: 50%.

Report score: 30%.

Algorithm performance: 20%. (The score of the effect is distributed to 12-20 points according to the ranking.)

An additional file, “contribution.pdf,” should be attached to describe the contribution of each member in the group and arrange the names according to the weight of their contributions. This file will serve as a reference for grading each member.

ABR Paper List

The following is a list of the ABR-related paper, including but not limited to:

1. Adaptation algorithm for adaptive streaming over HTTP. (2012)

2. Towards agile and smooth video adaptation in dynamic HTTP streaming. (2012)

3. Rate adaptation for dynamic adaptive streaming over HTTP in content distributionnetwork. (2012)

5. Probe and adapt: Rate adaptation for HTTP video streaming at scale. (2014)

6. A buffer-based approach to rate adaptation: Evidence from a large video streamingservice. (2014)

7. A Control-Theoretic Approach for Dynamic Adaptive Video Streaming over HTTP.(2015)

8. Machine learning based rate adaptation with elastic feature selection for HTTPbased streaming. (2015)

…

0x04 Environment and Programming Entry

After writing an ABR algorithm it can be tested by first running python studentComm.py in one terminal window and then python simulator.py &lt;tracefile.txt&gt; &lt;manifestfile.json&gt; in another. studentComm.py is a simple communication layer between the simulator and the student example code inside of studentcodeExample.py . Test conditions can be manipulated by modifying the tracefile.txt and manifestfile.json files. Their specifications are detailed below.

Run the Example

For example, from the main directory, and run the following two command in two different terminal:

python studentComm.py

python simulator.py inputs/traceHD.txt inputs/manifestHD.json

Trace Files

The trace file dictates the bandwidth throughout a test run. On each line the 1st value represents the Video Time threshold where a bandwidth switch occurs and the 2nd value

represent the bandwidth value it will switch to. The first and second value must be separated by a single space.

A tracefile always must have a value for time 0. There can be as many or as few values as needed. The last bandwidth will describe the bandwidth until the test finishes. For example:

Manifest

The manifest file dictates other parameters such as chunks information, available bitrate, buffer size, and much more. rand_sizes.py can be used to quickly change chunk size information. It uses a normal distribution to randomly generate chunk sizes for a more natural test case.

Here is an example configuration for a Manifest file:

Grader

After writing an ABR algorithm in studentcodeEX.py, the grader can be ran using: python grader.py

The grader will look for a directory named “tests” within the current directory. Within tests should be multiple directories, each representing a testcase. The name of a testcase directory is arbitrary and will correspond to the name of the test. Inside each testcase directory must be a manifest and trace file which will be run on the simulator.

Files Specification

Below is the file tree of the given environment zip file of this homework:

├───Classes //python classes used in the simulator and grader

├───inputs //inputs files used for single use testing

├───papers //some paper references used for the ABR algorithms

├───tests //tests that grader will run

│ ├───testALThard //test that have a unstable bandwidth that confuses ABR algos

│ ├───testALTsoft //test that have a lot of alternating bandwidth

│ ├───testHD //test that have high quality bandwidth and other params

│ ├───testHDmanPQtrace //test that have high quality bandwidth but low params │ ├───testPQ //test that have low quality bandwidth and param, will rebuffer.

│ └───…

├───grader.py //python file that graded the ABR algorithm via QOE

├───rand_sizes.py //python helper file use to generate chunk sizes

├───simulator.py //the simulator that generate parameters from text and json files

├───studentcodeExample.py //the file where that contains the student entrypoint

└───studentComm.py //the program the student will call to invoke their ABR algorithm

Entry

As aforementioned, studentComm.py is the test entry to example code inside of studentcodeExample.py .You need to implement your own studentcode_119010001.py(replace with your ID), and change the entry in studentComm.py to your code.

0x05 Submission Details

Please compress all files in the file structure root folder into a single zip file and name it using your student id as the code showing below and above, for example, Assignment_119010001.zip.

The report should be submitted in the format of pdf, together with your source code, (and contribution.pdf for Task-2). Format mismatch would cause grade deduction. Violation against each format requirements will lead to 5 demerit points.

If you use third-party python library, please install them in conda environment, and remember to export your conda environment by using command conda list -e &gt; req.txt . Please attach this environment file in the zip file.

We don’t recommand to use other languages. However, if you still want to use language rather than python(C/C++/Java/Go, etc.), remember the entry is fixed and call your program from python (such as using ctypes library to call C function from Python). Please make sure your program can execute directly and got result without any errors.

Also, remember to attach all of the source code, compile files, excutable files, and list all installed-library/installed-command you need.

We take your honesty seriously. Please write your own code.

0x06 References:

2. Huang T Y, Johari R, McKeown N, et al. A buffer-based approach to rate adaptation: Evidence from a large video streaming service[C]//Proceedings of the 2014 ACM conference on SIGCOMM. 2014: 187-198.

(https://www.cloudflare.com/learning/video/what-is-adaptive-bitrate-streaming/).

6. Sydney Whalen. Adaptive Bitrate Streaming: How It Works and Why It Matters (Update).

(https://en.wikipedia.org/wiki/Adaptive_bitrate_streaming)

(https://github.com/henryhxu/CSCI4430-ESTR4120)

(https://github.com/zpeats/50863_ABR_Lab)

12. Akhshabi S, Begen A C, Dovrolis C. An experimental evaluation of rate-adaptation algorithms in adaptive streaming over HTTP[C]//Proceedings of the second annual ACM conference on Multimedia systems. 2011: 157-168.

13. Miller K, Quacchio E, Gennari G, et al. Adaptation algorithm for adaptive streaming over HTTP[C]//2012 19th international packet video workshop (PV). IEEE, 2012: 173-178.

14. Tian G, Liu Y. Towards agile and smooth video adaptation in dynamic HTTP streaming[C]//Proceedings of the 8th international conference on Emerging networking experiments and technologies. 2012: 109-120.

15. Liu C, Bouazizi I, Hannuksela M M, et al. Rate adaptation for dynamic adaptive streaming over HTTP in content distribution network[J]. Signal Processing: Image Communication, 2012, 27(4): 288-311.

17. Li Z, Zhu X, Gahm J, et al. Probe and adapt: Rate adaptation for HTTP video streaming at scale[J]. IEEE Journal on Selected Areas in Communications, 2014, 32(4): 719-733.

18. Yin X, Jindal A, Sekar V, et al. A control-theoretic approach for dynamic adaptive video streaming over HTTP[C]//Proceedings of the 2015 ACM Conference on Special Interest Group on Data Communication. 2015: 325-338.

19. Chien Y L, Lin K C J, Chen M S. Machine learning based rate adaptation with elastic feature selection for HTTP-based streaming[C]//2015 IEEE International Conference on Multimedia and Expo (ICME). IEEE, 2015: 1-6.
