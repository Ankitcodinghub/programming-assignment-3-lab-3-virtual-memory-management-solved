# programming-assignment-3-lab-3-virtual-memory-management-solved
**TO GET THIS SOLUTION VISIT:** [Programming Assignment #3 (Lab 3): Virtual Memory Management Solved](https://www.ankitcodinghub.com/product/programming-assignment-3-lab-3-virtual-memory-management-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;10771&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;4&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (4 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Programming Assignment #3   (Lab 3): Virtual Memory Management Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
            5/5 - (4 votes)    </div>
    </div>
In this lab/programming assignment you will implement/simulate the operation of a Virtual Memory Manager that maps the virtual address spaces of multiple processes onto physical frames. The assignment will assume multiple processes, each with its own virtual address space of 64 virtual pages. As the sum of all virtual pages in all virtual address space may exceed the number of physical pages of the simulated system paging needs to be implemented. The number of physical page frames varies and is specified by a program option, but assume you have to support 128 frames (No more, but certainly less). Implementation is to be done in C/C++. Please submit your source including a Makefile as a single compressed file via NYU classes.

&nbsp;

<strong><u>INPUT SPECIFICATION:</u> </strong>

&nbsp;

The input to your program will be a comprised of:

<ol>
<li>the number of processes (processes are numbered starting from 0)</li>
<li>a specification for each process’ address space is comprised of</li>
<li>the number of virtual memory areas (aka VMAs)</li>
<li>specification for each said VMA comprises of 4 numbers:</li>
</ol>
“starting_virtual_page&nbsp;&nbsp; ending_virtual_page&nbsp; write_protected[0/1] filemapped[0/1]”

&nbsp;

Following is a sample input with two processes. First line not starting with a ‘#’ is the number of processes. Each process in this sample has two VMAs. <strong><u>Note:</u></strong> <strong>ALL </strong>lines starting with ‘#’ must be ignored and are provided simply for documentation and readability. In particular, the first few lines are references that <em>document </em>how the input was created, though they are irrelevant to you.

&nbsp;

<strong>#process/vma/page reference generator </strong>

<strong>#&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; procs=2 #vmas=2 #inst=100 pages=64 %read=75.000000 lambda=1.000000 </strong>

<strong>#&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; holes=1 wprot=1 mmap=1 seed=19200 </strong>

<strong>2 </strong>

<strong>#### process 0 </strong>

<strong># </strong>

<strong>2 </strong>

<strong>0 42 0 0 </strong>

<strong>43 63 1 0 </strong>

<strong>#### process 1 </strong>

<strong># </strong>

<strong>2 </strong>

<strong>0 17 0 1 20 63 1 0</strong>

&nbsp;

Since it is required for VMAs of single address space to not overlap, this property is guaranteed for all provided input files. However, there can potentially be holes between VMAs, which means that not all virtual pages of an address space are valid (i.e. assigned to a VMA). Each VMA is comprised of 4 numbers.

<em>start_vpage</em>:

<em>end_vpage</em>:&nbsp; (note the VMA has&nbsp;&nbsp;&nbsp; (end_page – start_vpage + 1)&nbsp;&nbsp; virtual pages <em>write_protected</em>:&nbsp;&nbsp; binary whether the VMA is write protected or not&nbsp; <em>file_mapped</em>: binary to indicated whether the VMA is mapped to a file or not

&nbsp;

The process specification is followed by a sequence of “instructions” and optional comment lines (see following example). An instruction line is comprised of a character (‘c’, ‘r’, or ‘w’) followed by a number.

“c &lt;procid&gt;” specifies that a context switch to process #&lt;procid&gt; is to be performed. It is guaranteed that the first instruction will always be a context switch instruction.

“r &lt;vpage&gt;” implies that a load/read operation is performed on said virtual page. “w &lt;vpage&gt;” implies that a store/write operation is performed on said virtual page.

&nbsp;

<strong>#</strong> <strong>#### instruction simulation ###### c 0 r 32 w 9 r 0 r 20 r 12 </strong>

&nbsp;

You can assume that the input files are well formed as shown above, so fancy parsing is not required. Just make sure you take care of the ‘#’ comment lines.

&nbsp;

<strong><u>DATA STRUCTURES:</u>&nbsp; </strong>

<strong>&nbsp;</strong>

To approach this assignment, read in the specification and create processes with its list of <em>vma</em>s and a <em>page_table</em> that represents the translations from virtual pages to physical frames for that process.

&nbsp;

In addition, you must define a global <em>frame_table</em> that each operating system maintains to describe the usage of each of its physical frames and where you maintain backward mappings to the address space(s) and the vpage that maps a particular frame (In this assignment a frame can only be mapped by at most one PTE at a time).

&nbsp;

A page table naturally must contain exactly 64 page table entries (PTE). A PTE is comprised of the PRESENT/VALID, WRITE_PROTECT, MODIFIED, REFERENCED and PAGEDOUT bits and an index to the physical frame (in case the pte is present). This information can and <strong>should</strong> be implemented as a single 32-bit value or as a bit structures (likely easier). It cannot be a structure of multiple integer values that collectively are larger than 32-bits. (see <u><a href="http://www.cs.cf.ac.uk/Dave/C/node13.html">http://www.cs.cf.ac.uk/Dave/C/node13.html</a></u> (BitFields) or&nbsp; <u><a href="http://www.catonmat.net/blog/bit-hacks-header-file/">http://www.catonmat.net/blog/bit</a><a href="http://www.catonmat.net/blog/bit-hacks-header-file/">–</a><a href="http://www.catonmat.net/blog/bit-hacks-header-file/">hacks</a><a href="http://www.catonmat.net/blog/bit-hacks-header-file/">–</a><a href="http://www.catonmat.net/blog/bit-hacks-header-file/">header</a><a href="http://www.catonmat.net/blog/bit-hacks-header-file/">–</a><a href="http://www.catonmat.net/blog/bit-hacks-header-file/">file/</a></u> as an example, I highly encourage you to use this technique).

Assuming that the maximum number of frames is 128, which equals 7 bits&nbsp; and the mentioned 5 bits above, you effectively have 32-12 = 20 bits for your own usage in the pagetable. You can use these bits as will (e.g. remembering whether a PTE is file mapped or not).

&nbsp;

<strong><u>SIMULATION and IMPLEMENTATION:</u>&nbsp; </strong>

&nbsp;

During each instruction you simulate the behavior of the hardware and hence you must check that the page is present. A special case is the ‘c’ (context switch) instruction which simply changes the current process and current page table pointer.

&nbsp;

<strong>Structure of the simulation </strong>

&nbsp;

The structure of the simulation should be something like the following:

&nbsp;

class Pager {&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; virtual frame* determine_victim_frame();

};

&nbsp;

Frame *get_frame() {

Frame *frame = allocate_frame_from_free_list();

if(frame == NULL) frame = THE_PAGER-&gt;determine_victim_frame();&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return frame;

}

&nbsp;

while (get_next_instruction(&amp;operation, &amp;vpage)) {

pte = &amp;current_process.page_table[vpage];&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; // done by hardware in reality&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if (pte-&gt;notpresent) {

Frame *newframe = get_frame();

//-&gt; figure out if/what to do with old frame if it was mapped

//&nbsp;&nbsp; see general outline in MM-slides under Lab3 header

//&nbsp;&nbsp; see whether and how to bring in the content of the access page.

}

// simulate instruction execution by hardware by updating the PTE bits

Update_pte(read/modify/write) bits based on operations.

}

&nbsp;

&nbsp;

If the page is not present, as indicated by the associated PTE’s valid/reference bit, the hardware would raise a page fault exception. Here you just simulate this by calling your (operating system’s) pagefault handler. In the pgfault handler you&nbsp; first determine that the <em>vpage</em> can be accessed, i.e. it is part of one of the VMAs. If not, a SEGV output line must be created and you move on to the next instruction. If it is part of a VMA then the page must be instantiated, i.e. a frame must be allocated, assigned to PTE belonging to the vpage of this instruction (i.e. <em>currentproc-&gt;pagetable[vpage].frame = allocated_frame</em> ) and then populated with the proper content. The population depends whether this page was previously paged out (in which case the page must be brought back from the swap space (“IN”) or (“FIN” in case it is a memory mapped file). If the vpage was never swapped out and is not file mapped, then by definition it still has a zero filled content and you issue the “ZERO” output.

&nbsp;

That leaves the allocation of frames. All frames initially are in a free “list”, which you can implement as an index to the frame_table (starting with 0) [ note once all frames are used in this assignment they are never returned to the free list ]. Once you run out of free frames, you must implement paging. We explore the implementation of several page replacement algorithms. Page replacement implies the identification of a victim page according to the algorithm’s policy. This should be implemented as a subclass of a general <em>Pager</em> class with essentially one virtual function&nbsp; “frame_t* (*select_frame)(void); “ that returns a victim frame. Once a victim frame has been determined, the victim frame must be unmapped from its user ( &lt;address space:vpage&gt;), i.e. its entry in the owning process’s page_table must be removed&nbsp; (“UNMAP”), however you must remember the state of the bits. If the page was modified, then the page frame must be paged out to the swap device (“OUT”) or in case it was file mapped written back to the file (“FOUT”). Now the frame can be reused for the faulting instruction. First the PTE must be reset (note once the PAGEDOUT flag is set it will never be reset as it indicates there is content on the swap device) and then the PTE’s frame must be set.

&nbsp;

Classes for every paging algorithm should derive from a base Pager class and there should be no replication of the simulation code. If you need a special functions (e.g. HW LRU), create an empty base function and overwrite in the specific pager subclass. This will allow adding new classes.

&nbsp;

At this point it is guaranteed, that the vpage is backed by a frame and the instruction can proceed in hardware (with the exception of the SEGV case above) and you have to set the REFERENCED and MODIFIED bits based on the operation. In case the instruction is a write operation and the PTE’s write protect bit is set (which it inherited from the VMA it belongs to) then a SEGPROT output line is to be generated. The page is considered referenced but not modified in this case.

&nbsp;

Your code must actively maintain the PRESENT (aka valid), MODIFIED, REFERENCED, and PAGEDOUT bits and the frame index in the pagetable’s pte. The frame table is NOT updated by the simulated hardware as hardware has no access to the frame table. Only the pagetable entry (pte) is updated just as in real operating systems and hardware.

&nbsp;

The following page replacement algorithms are to be implemented (letter indicates option (see below)):

&nbsp;

<table width="420">
<tbody>
<tr>
<td width="228">Algorithm</td>
<td width="192">Based on Physical Frames</td>
</tr>
<tr>
<td width="228">FIFO</td>
<td width="192">f</td>
</tr>
<tr>
<td width="228">Second-Chance (derivative of FIFO)</td>
<td width="192">s</td>
</tr>
<tr>
<td width="228">Random</td>
<td width="192">r</td>
</tr>
<tr>
<td width="228">NRU (Not Recently Used)</td>
<td width="192">n</td>
</tr>
<tr>
<td width="228">Clock</td>
<td width="192">c</td>
</tr>
<tr>
<td width="228">Aging</td>
<td width="192">a</td>
</tr>
</tbody>
</table>
&nbsp;

The page replacement should be generic and the algorithms should be special instances of the page replacement class to <strong>avoid “switch/case statements” in the simulation of instructions</strong>. Use object oriented programming and inheritance.

&nbsp;

When a virtual page is replaced, it must be first unmapped and then optionally paged out or written back to file. While you are not effectively implementing these operations you still need to track them and create entries in the output (see below).

&nbsp;

Since all replacement algorithms are based on frames and the reference and modified bits are only maintained in the page tables of processes you need access to the PTEs. To be able to do that you should keep track of the inverse mapping:

(frame –&gt; &lt;proc-id,vpage&gt;) inside each frame’s frame table entry.

&nbsp;

&nbsp;

You are to create the following output if requested by an option (see at options description):

&nbsp;

<table width="566">
<tbody>
<tr>
<td width="222">78: ==&gt; r 2

UNMAP 1:42

OUT

IN

MAP 26

&nbsp;

Output 1
</td>
<td width="240">69: ==&gt; r 37

UNMAP 0:35

IN

MAP 18

&nbsp;

&nbsp;

Output 2
</td>
<td width="104">75: ==&gt; w 57&nbsp; UNMAP 2:58

ZERO

MAP 17

&nbsp;

&nbsp;

Output 3
</td>
</tr>
</tbody>
</table>
For instance in Output 1 Instruction 78 is a read operation on virtual page 2 of the current process. The replacement algorithms selected physical frame 26 that was used by virtual page 42 of process 1 (1:42) and hence first has to <strong>UNMAP</strong> the virtual page 42 of process 1 to avoid further access, then because the page was dirty (modified) (this would have been tracked in the PTE) it pages the page <strong>OUT</strong> to a swap device with the (1:26) tag so the Operating system can find it later when process 1 references vpage 42 again (note you don’t implement the lookup). Then it pages <strong>IN</strong> the previously swapped out content of virtual page 2 of the current process (note this is where the OS would use &lt;current-process-id : vpage&gt; tag to find the swapped out page) into the physical frame 26, and finally maps it which makes the PTE_2 a valid/present entry and allows the access. Similarly, in output 2 a read operation is performed on virtual page 37. The replacement selects frame 18 that was mapped by process_0’s vpage=35. The page is not paged out, which indicates that it was not dirty/modified since the last mapping. The virtual page 37 is then paged in to physical frame 18 and finally mapped. In output 3 you see that frame 17 was selected forcing the unmapping of its current user process_2, page 58, the frame is zeroed (hence no virtual page number in the output), which indicates that the page was never paged out or written back to file (though it might have been unmapped previously see output 2). An operating system must zero pages on first access (unless filemapped) to guarantee consistent behavior. In the case of filemapped virtual pages (i.e. part of filemapped VMA) even the initial content must be loaded from file.

&nbsp;

In addition your program needs to compute and print the summary statistics related to the VMM if requested by an option. This means it needs to track the number of instructions, segv, segprot, unmap, map, pageins (IN, FIN), pageouts (OUT, FOUT), and zero operations for each process. In addition you should compute the overall execution time in cycles, where maps and unmaps each cost 400 cycles, page-in/outs each cost 3000 cycles, file in/outs cost 2500 cycles, zeroing a page costs 150 cycles, a segv costs 240 cycles, a segprot costs 300 cycles and each access (read or write) costs 1 cycles and a context switch costs 121 cycles.

&nbsp;

Per process:

printf(“PROC[%d]: U=%lu M=%lu I=%lu O=%lu FI=%lu FO=%lu Z=%lu SV=%lu SP=%lu\n”,&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;proc-&gt;pid,

pstats-&gt;unmaps, pstats-&gt;maps, pstats-&gt;ins, pstats-&gt;outs,

pstats-&gt;fins, pstats-&gt;fouts, pstats-&gt;zeros,&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; pstats-&gt;segv, pstats-&gt;segprot);

All:

printf(“TOTALCOST %lu %lu %llu\n”, ctx_switches, inst_count, cost);

&nbsp;

If requested by an option you have to print the relevant content of the page table of each process and the frame table.

&nbsp;

PT[0]: * 1:RM- * * * 5:-M- * * 8:— * * # * * * * * * * * # * * * 24:— * * * # *

* * * * * * * * # * * * * * * * * * # * * # * * * # * * * * * * * *

FT: 0:1 0:5 0:24 0:8

PROC[0]: U=25 M=29 I=1 O=8 FI=0 FO=0 Z=28 SV=0 SP=0

TOTALCOST 1 31 52951

&nbsp;

Note, the cost calculation can overrun 2^32 and you must account for that, so use 64-bit counters. We will test your program with 1 Million instructions. Also the end calculations are tricky, so do them incrementally. Don’t add up 32-bit numbers and then assign to 64-bit. Add 32-bit numbers incrementally to the 64-bit counters, if you use 32-bit.

<strong>Execution and Invocation Format: </strong>

<strong>&nbsp;</strong>

Your program <strong>must</strong> follow the following invocation:

./mmu&nbsp; [-a&lt;algo&gt;]&nbsp; [-o&lt;options&gt;] [–f&lt;num_frames&gt;] inputfile&nbsp;&nbsp; randomfile&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (optional arguments in any order).

e.g. ./mmu –ac –o[OPFS] infile rfile selects the Clock Algorithm and creates output for operations, final page table content and final frame table content and summary line (see above). The outputs should be generated in that order if specified in the option string regardless how the order appears in the option string. <strong>We will grade the program with –oOPFS options</strong> (see below), change the page frame numbers and “diff” compare it to the expected output.

&nbsp;

The test input files and the sample file with random numbers are supplied. The random file is required for the Random algorithm and the NRU algorithm. Please reuse the code you have written for lab2, but note the difference in the modulo function which now indexes into [ 0, size ) vs previously ( 0, size ].

&nbsp;

In the Random replacement algorithm you compute the frame selected as with (size==num_frames) and in the NRU algorithm, you use the random function to select a random frame from the lowest class identified, in particular you should create the class by creating an array and then index into that array via the index = array[class][ rands[rofs] % num_pages_in_array[class] ]. As in the lab2 case, you increase the <em>rofs</em> and wrap around from the input file.

&nbsp;

<ul>
<li>The ‘O’ (ohhh) option shall generate the required output as shown in output-1/3.</li>
</ul>
&nbsp;

<ul>
<li>The ‘P’ (pagetable option) should print after the execution of all instructions the state of the pagetable: As a single line, you print the content of the pagetable pte entries as follows:</li>
</ul>
&nbsp;

0:RMS 1:RMS 2:RMS 3:R-S 4:R-S 5:RMS 6:R-S 7:R-S 8:RMS 9:R-S 10:RMS 11:R-S

12:R– 13:RM- # # 16:R– 17:R-S # # 20:R– # 22:R-S 23:RM- 24:RMS # # 27:R-S

28:RMS # # # # # 34:R-S 35:R-S # 37:RM- 38:R-S * # 41:R– # 43:RMS 44:RMS #

46:R-S * * # * * * # 54:R-S # * * 58:RM- * * # * *

&nbsp;

R (referenced), M (modified), S (swapped out) (note we don’t show the write protection bit as it is implied/inherited from the specified VMA. Pages that are not valid are represented by a ‘#’ if they have been swapped out (note you don’t have to swap out a page if it was only referenced but not modified), or a ‘*’ if it does not have a swap area associated with. Otherwise

(valid) indicates the virtual page index and RMS bits with ‘-‘ indicated that that bit is not set.

Note a virtual page, that was once referenced, but was not modified and then is selected by the replacement algorithm, does not have to be paged out (by definition all content must still be ZERO) and can transition to ‘*’.

&nbsp;

<ul>
<li>The ‘F’ (frame table option) should print after the execution and should show which frame is mapped at the end to</li>
</ul>
which &lt;pid:virtual page&gt; or ‘*’ if not currently mapped by any virtual page.

&nbsp;

FT: 0:32 0:42 0:4 1:8 * 0:39 0:3 0:44 1:19 0:29 1:61 * 1:58 0:6 0:27 1:34

&nbsp;

<ul>
<li>The ‘S’ option prints the summary line (“SUM …”) described above.</li>
<li>The ‘x’ options prints the current page table after each instructions (see example outputs) and this should help you significantly to track down bugs and transitions</li>
<li>The ‘y’ option is like ‘x’ but prints the page table of all processes instead.</li>
<li>The ‘f’ option prints the frame table after each instruction.</li>
<li>The ‘a’ option prints the “aging” information after each instruction for complex algorithms.</li>
</ul>
&nbsp;

We will not test or use the ‘-f’ ,’-a’ or the ‘-x,-y’ option during the grading. <strong>It is purely for your benefit to add these and compare with the reference program</strong>

&nbsp;

All scanning replacement algorithm, should start at frame[0].

&nbsp;

<strong><u>Please note</u></strong> you have to provide a modular design which separates the simulation (instruction by instruction) from the replacement policies. Use OO style of programming and think about what operations you need from a generic page replacement (which will define the API). A lack of doing a modular design with separated replacement policies and simulation will lead to a deduction of 5pts.

&nbsp;

<strong>FAQ: </strong>

&nbsp;

<strong>NRU</strong> requires that the REFERENCED-bit be periodically reset for all valid page table entries. The book suggest on every clock cycle. Since we don’t implement a clock interrupt, we shall reset the ref bits every 10<sup>th</sup> page replacement request before you implement the replacement operation (note these don’t include the initial page faults, only invocation for selecting a victim page).

&nbsp;

<strong>AGING</strong> requires to maintain the age-bit-vector. In this assignment please assume a 32-bit counter (vector). It is implemented on every page replacement request.

&nbsp;

The <em>pagetable</em> and <em>frametable </em>output is generated AFTER the instruction is executed, so the output becomes the state seen prior to executing the next instruction.

&nbsp;

How do I provide <strong>optional argument</strong>s in arbitrary order ?

Please read:&nbsp;&nbsp; <u><a href="http://www.gnu.org/software/libc/manual/html_node/Example-of-Getopt.html">http://www.gnu.org/software/libc/manual/html_node/Example</a><a href="http://www.gnu.org/software/libc/manual/html_node/Example-of-Getopt.html">–</a><a href="http://www.gnu.org/software/libc/manual/html_node/Example-of-Getopt.html">of</a><a href="http://www.gnu.org/software/libc/manual/html_node/Example-of-Getopt.html">–</a><a href="http://www.gnu.org/software/libc/manual/html_node/Example-of-Getopt.html">Getopt.html</a></u>

&nbsp;

What data structures do I maintain:

You must maintain a single level pagetable (struct PTE page_table[64]) per process and a global frametable[num_frames] Note that reference and modified etc can ONLY be maintained in the pagetables as hardware will only update those in real life. <strong>The frametable is an OS structure with one entry to represent/describe per physical frame</strong>. PTE bits ( Reference, Modified, et. al. are <strong>NOT</strong> maintained in the frametable)

&nbsp;

<strong>Provided Inputs </strong>

&nbsp;

The submission comes with a few generated inputs that you can use to address implementation in an incremental step. Each input is characterized by how many processes, how many maximum vmas per process, how many maximum write protected vmas per process, whether there is a filemapped vma and maximum numbers of vma holes might exist for a process.

&nbsp;

<table width="389">
<tbody>
<tr>
<td width="57">Input File</td>
<td width="48">#inst</td>
<td width="50">#procs</td>
<td width="81">#vmas

(max)
</td>
<td width="51">Write- protect</td>
<td width="57">File-

mapped
</td>
<td width="45">Holes</td>
</tr>
<tr>
<td width="57">in1</td>
<td width="48">30</td>
<td width="50">1</td>
<td width="81">1</td>
<td width="51">0</td>
<td width="57"></td>
<td width="45"></td>
</tr>
<tr>
<td width="57">in2</td>
<td width="48">30</td>
<td width="50">1</td>
<td width="81">1</td>
<td width="51">0</td>
<td width="57"></td>
<td width="45"></td>
</tr>
<tr>
<td width="57">in3</td>
<td width="48">100</td>
<td width="50">1</td>
<td width="81">4</td>
<td width="51">0</td>
<td width="57"></td>
<td width="45"></td>
</tr>
<tr>
<td width="57">in4</td>
<td width="48">100</td>
<td width="50">1</td>
<td width="81">5</td>
<td width="51">2</td>
<td width="57"></td>
<td width="45"></td>
</tr>
<tr>
<td width="57">in5</td>
<td width="48">100</td>
<td width="50">1</td>
<td width="81">5</td>
<td width="51">0</td>
<td width="57">1</td>
<td width="45"></td>
</tr>
<tr>
<td width="57">in6</td>
<td width="48">100</td>
<td width="50">1</td>
<td width="81">5</td>
<td width="51">2</td>
<td width="57"></td>
<td width="45">2</td>
</tr>
<tr>
<td width="57">in7</td>
<td width="48">200</td>
<td width="50">2</td>
<td width="81">2</td>
<td width="51"></td>
<td width="57"></td>
<td width="45"></td>
</tr>
<tr>
<td width="57">in8</td>
<td width="48">200</td>
<td width="50">2</td>
<td width="81">3</td>
<td width="51">1</td>
<td width="57">1</td>
<td width="45"></td>
</tr>
<tr>
<td width="57">in9</td>
<td width="48">1000</td>
<td width="50">3</td>
<td width="81">4</td>
<td width="51">1</td>
<td width="57">1</td>
<td width="45">2</td>
</tr>
<tr>
<td width="57">in10</td>
<td width="48">10000</td>
<td width="50">4</td>
<td width="81">6</td>
<td width="51">2</td>
<td width="57">1</td>
<td width="45">2</td>
</tr>
</tbody>
</table>
&nbsp;

It is suggested that you follow this approach

<ol>
<li>read the input creating your processes and their respective vmas and print them out again, to ensure you read properly.</li>
<li>implement the features for a single process first (in1..in6) and implement one algorithm (e.g. fifo).</li>
<li>add the basic features for context switching (in7..in8) and then expand to other algorithms</li>
<li>Finally, try the more complex input files (in9..in10).</li>
</ol>
&nbsp;

Sample output files are provided as a *.tz (tar’d and <span style="text-decoration: line-through;">feathered </span>compressed) for each input and each algorithm for two frame number scenarios –f16 and –f32 à 10 * 2 * 6 à 120 files. If you need more you can generate your own outputs using the reference program on the cims account (under <em>~frankeh/Public/mmu) </em>for different frame numbers.

&nbsp;

I also provide a ./runit.sh and a ./gradeit.sh.&nbsp; ( change the INPUTS and ALGOS in both to limit what you want to test) ./runit.sh &lt;inputs_dir&gt; &lt;output_dir&gt; &lt;executable&gt;

./gradeit.sh &lt;refout_dir&gt; &lt;output_dir&gt;&nbsp;&nbsp;&nbsp; # will generate a summary statement and &lt;output_dir&gt;/LOG file for more details

Look at the LOG file and it shows the “diff command” for those files that failed and even if the TOTALCOST are the same there are differences elsewhere. Remove the ‘-q’ flag in the diff command of the LOG and run manually.

&nbsp;

<strong><u>OTHER STUFF:</u> </strong>

&nbsp;

The following data structures should&nbsp; somewhat find their way into your program:

&nbsp;
