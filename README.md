Download Link: https://assignmentchef.com/product/solved-cs20a-quiz-2
<br>
Cautionary Rant: It is a good idea to check your work by actually programming any problem.  But, it is critically important to complete these, or any exercise, without the aid of your computer <strong>first</strong>.  You will not have access to a computer during the exam or during most technical interviews with any large software development company.

<strong>Problem 1: Doubly Linked List Class </strong>

We will build a <u>sorted</u> doubly linked list. The following shows an example of a list with 4 elements, where the nodes are sorted in the increasing order of their values. The m_prev pointer of the head node and m_next pointer of the tail node both point to nullptr. If the list is empty, head and tail pointers both point to nullptr.

Assume the following declaration of Node structure and SortedLinkedList class.




<table width="582">

 <tbody>

  <tr>

   <td colspan="2" width="204">struct Node {</td>

   <td rowspan="2" width="378">class SortedLinkedList { public:SortedLinkedList();       bool insert(const int &amp;value);        const Node *search(const int &amp;value) const;void remove(Node *node);  int size() const { return m_size; }          void printIncreasingOrder() const;private:Node * m_head;         Node *m_tail;int m_size;} </td>

  </tr>

  <tr>

   <td width="48">   }; </td>

   <td width="156">int value;  Node *prev;Node *next;</td>

  </tr>

  <tr>

   <td width="48"></td>

   <td width="156"></td>

   <td width="378"></td>

  </tr>

 </tbody>

</table>




<ol>

 <li>Implement SortedLinkedList().</li>

</ol>

SortedLinkedList::SortedLinkedList() {

}

<ol>

 <li>Implement insert(). If a node with the same value is already in the list, do not insert a new node. Return true if a new node is successfully inserted, and return false otherwise.</li>

</ol>

bool SortedLinkedList::insert(const int &amp;value) {

<ol>

 <li>Implement search(), which returns the pointer to the node with the specified value.</li>

</ol>




const Node *SortedLinkedList::search(const int &amp;value) const {




<ol>

 <li>Implement remove(). Assume node is either nullptr (in which case you would simply return) or a valid pointer to a Node in the list, as found in search().</li>

</ol>

LinkedList::remove(Node *node) {

<ol>

 <li>Implement printIncreasingOrder(), which prints the values stored in the list in the increasing order, one value in each line.</li>

</ol>

void SortedLinkedList::printIncreasingOrder() const {

<ol>

 <li>Program your implementation in a single file named sdll.h and include that with your quiz 2 submission archive.</li>

</ol>




<strong>Problem 2: Recursion </strong>




<ol>

 <li>Write a recursive function that computes base<sup>exp </sup>(base raised to the power of exp). What is the BigO of this function?</li>

</ol>

int recursivePow(int base, int exp) {

<ol>

 <li>Write a function powerThree that, given a non-negative number n, returns 3<sup>n</sup> (3^n, or “3 raised to power n”) <u>recursively</u>, assuming 3<sup>n</sup> is something that can be represented as an integer. Do <u>not</u> use a loop, and do not use the character ‘*’ anywhere in your code. What is the Big-O of this function?</li>

</ol>

int powerThree(int n) {

<h1>Problem 3: Big-O</h1>

<ol>

 <li>Suppose Algorithm A and B perform the same task. For any given input size n, algorithm A executes in f(n)=0.003n2 operations, and algorithm B executes f(n)=250n operations. Specifically, when does Algorithm A perform better than B?</li>

 <li>An algorithm that is O(n<sup>2</sup>) takes 10 seconds to complete when n=100. How long would you expect it to take when n=500?</li>

 <li>What is the Big-O of the following code segment:</li>

</ol>

for (int i = 0; i &lt; n; i++)

for (int j = 0; j &lt; 4 * i; j++)                                         sum++;

<ol>

 <li>What is the Big-O of the following function?</li>

</ol>

int gobidygoop(int n, int p) {  int ac = 1;

for (int i = 0; i &lt; n; i++) {

int k = p;

while (k &gt; 1) {

ac *= i + k;           k /= 4;

}

}

}

<ol>

 <li>Consider the following pseudo code:</li>

</ol>

Get value for n

Set the value of k to 1

While k is less than or equal to n

Set the value of j to twice of k

While j is greater or equal to 1

Print the value of j

Set the value of j to one half its former value;    Increase k by 1

What is the Big-O of this pseudocode? What does this print if n is 4?

<strong>Problem 5: Sorting </strong>

<strong> </strong>

<ol>

 <li>Fill out the following table or sorting properties, if there is no special condition for a particular case then leave it blank:</li>

</ol>

<table width="689">

 <tbody>

  <tr>

   <td width="136">Sorting Algorithm</td>

   <td width="111">Selection</td>

   <td width="111">Insertion</td>

   <td width="111">Bubble</td>

   <td width="111">Quick</td>

   <td width="111">Merge</td>

  </tr>

  <tr>

   <td width="136">Average  Complexity</td>

   <td width="111"> </td>

   <td width="111"> </td>

   <td width="111"> </td>

   <td width="111"> </td>

   <td width="111"> </td>

  </tr>

  <tr>

   <td width="136">Worse  Complexity</td>

   <td width="111"> </td>

   <td width="111"> </td>

   <td width="111"> </td>

   <td width="111"> </td>

   <td width="111"> </td>

  </tr>

  <tr>

   <td width="136">Condition for Worse</td>

   <td width="111"> </td>

   <td width="111"> </td>

   <td width="111"> </td>

   <td width="111"> </td>

   <td width="111"> </td>

  </tr>

  <tr>

   <td width="136">Best  Complexity</td>

   <td width="111"> </td>

   <td width="111"> </td>

   <td width="111"> </td>

   <td width="111"> </td>

   <td width="111"> </td>

  </tr>

  <tr>

   <td width="136">Condition for Best</td>

   <td width="111"> </td>

   <td width="111"> </td>

   <td width="111"> </td>

   <td width="111"> </td>

   <td width="111"> </td>

  </tr>

 </tbody>

</table>




<ol>

 <li>Sort the following array using the Mergesort algorithm. Show each recursive step, including the merge.</li>

</ol>

<table width="221">

 <tbody>

  <tr>

   <td width="29">99</td>

   <td width="29">16</td>

   <td width="23">3</td>

   <td width="29">19</td>

   <td width="29">13</td>

   <td width="23">0</td>

   <td width="29">13</td>

   <td width="29">12</td>

  </tr>

 </tbody>

</table>


