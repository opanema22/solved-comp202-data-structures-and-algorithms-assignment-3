Download Link: https://assignmentchef.com/product/solved-comp202-data-structures-and-algorithms-assignment-3
<br>
<h1> This programming assignment will test your knowledge and your implementation abilities of what you have learned in the Trees, Binary Search Trees and Priority Queues parts of the class.</h1>

This homework must be completed individually. Discussion about algorithms and data structures are allowed but group work is not. <strong>Coming up with the same algorithm and talking about the ways of implementation leads to very similar code which is treated as plagiarism! </strong>Discuss carefully. Any academic dishonesty, which includes taking someone else’s code or having another person doing the assignment for you will not be tolerated. <strong>By submitting your assignment, you agree to abide by the Ko¸c University codes of conduct.</strong>

<h2>Description</h2>

The assignment will have two parts. The first part of the assignment requires you to implement a <em>Binary Search Tree </em>to be used as a map data structure with a few additional operations, implement a <em>Array Based Heap </em>and modify a BST. The last two will be used as a <em>Priority Queue</em>. The second part requires you to implement a phonebook as a table using your own binary search tree.

<h3>Part I: Implementing the Data Structures</h3>

You are going to implement a binary search tree which implements a given binary search tree interface and a given map interface. You are also given an adaptable priority queue interface. This is going to be implemented by an array-based heap and a binary search tree based priority queue, which also extends the previous binary search tree. The details of these interfaces will not be given here due to the comments in the files. <strong>Feel free to contact us if anything is unclear</strong>. You are additionally given additional classes that will help with the implementation.

As mentioned above, the code has comments about the assignment and the desired functionality. Majority of what you need to do is actually in these comments so make sure you read them carefully. You are provided with a compressed file which contains following files. Bold ones are the ones you need to modify and they are placed under the <em>code </em>folder, with the rest under <em>given</em>.

<ul>

 <li><em>java</em>: This file defines a simple map interface. Even though you do not need to modify this, make sure you read the comments in detail. It is pretty straight forward.</li>

 <li><em>java</em>: This file includes the iBinarySearchTree interface, which describes the desired binary search tree ADT. Even though you do not need to modify this, make sure you read the comments in detail.</li>

 <li><em>java</em>: This file includes the Entry class that describes a <em>Key-Value </em>pair. Certain useful methods are implemented for you. This will form the basis of your binary tree nodes and be used in the priority queues. You should take a look at its functions but do not modify it.</li>

 <li><em>java</em>: This file includes the BinaryTreeNode class which is used in the binary tree as nodes. It extends the Entry class. You are free to design and implement it however you want.</li>

 <li><em>java</em>: This is where one of the main data structures of the assignment, the BinarySearchTree class, should be implemented. It extends both the iBinarySearchTree and the iMap interfaces. You should implement this class and the BinaryTreeNode class in conjunction.</li>

 <li><em>java</em>: This file defines the iAdaptablePriorityQueue interface, which describes an adaptable priority queue interface. As with the other interface files, make sure to go over the comments. There is one important point, its operations assume that both the keys and the values are unique. This is done to make the assignment easier but it is not very realistic. If you ever need something like this in real life, keep this in mind! Another point is that the adaptations require you to find the right entries. This is slightly different than the <em>Position </em>concept we have seen, i.e., to change keys or values we find the relevant entry but do not store indiviual entries.</li>

 <li><em>java</em>: This file defines the binary search tree based priority queue class BSTBasedPQ.</li>

</ul>

It extends the BinarySearchTree class and implements the iAdaptablePriorityQueue interface. Do not try to create heap behavior but think about how to use a BST as a priority queue. Hint: There is a <em>O</em>(<em>h</em>) way to get to the minimum element!

<ul>

 <li><em>java</em>: This is where the other main data structure of the assignment, the ArrayBasedHeap class, should be implemented. It extends the iAdaptablePriorityQueue interface. We suggest that you first implement the array based binary tree functionality (no interface given but you can get inspiration from the available interfaces/classes), then add heap functionality. Make sure that this actually behaves as a heap and not a sorted list!</li>

 <li><em>java</em>: This file has the autograding for your data structures implementations. Run this to see your grade and errors.</li>

 <li><em>java</em>: An implementation of an order-book based on your priority queue implementations. This will be used as an “on the job” testing of your code. It simulates an order book for a single “item”. It reads the orders under the exchange folders and updates the priority queues. You can directly call the main function of this code for debugging. The <em>Exchange </em>folder contains small amount of orders to help you debug. Your code will be tested on the other two exchange folders. Autograder code calls a method under this file to create output files (e.g. <em>student </em><em>heap Exchange2 output.txt</em>) which are then compared to reference files, <em>Exchange2 output.txt </em>and <em>Exchange3 output.txt</em>. Feel free to ask about its implementation in person but we are not going to delve into the details here.</li>

 <li><em>java</em>: This file implements the comparators that are used in the assignment. You do not need to touch this or even go over it unless you are curious.</li>

 <li><em>java</em>: This file provides functionality to generate random data. You do not need to worry about it.</li>

 <li><em>java</em>: This file includes utility functions. Do not worry about it, you will not need to use anything from this file in this assignment.</li>

</ul>

<h3>Part II: Phonebook Application</h3>

You are asked to implement a phone book in the second part of the assignment. The phone book stores contact information and is efficiently searchable (In this context, efficient means not iterating over all the entries!) using two keys; contact name and contact number. In addition, it should be searchable by e-mail (not necessarily efficiently). We will go over how to do it in the class (Hint: Tables) before the submission deadline. <strong>You are only allowed to use your own tree implementation as a map in this second part!</strong>. My suggestion is for you to use two binary search trees, one for the contact name and the other for the contact number. All the rest are in the comments. The relevant files are:

<ul>

 <li><em>java</em>: This file has the ContactInfo class that you should store as your values. You do not need to touch this but should go over it.</li>

 <li><em>java</em>: This file includes the PhoneBook class which you need to complete based on the description given in this document and the comments in the file. To make things easier, you can assume that the name and numbers will be unique. (Note that we have gone over how to handle non-unique keys in the class. Hint: Multimaps). Other than only being allowed to use your own tree data structures, feel free to implement this class in any way you want.</li>

 <li><em>java</em>: This file contains the code for generating output using your phone-book implementation. It uses the <em>database.txt </em>to fill your phone-book and <em>query.txt </em>to perfrom operations on it. It generates a file named <em>student phonebook output.txt </em>to be compared with the provided <em>phonebook </em><em>output.txt </em>file. You can run this file separately as well. We are not going to delve into it how it works here but you can figure out how it works by looking at the code if needed. Feel free to create your own query and database files if the given ones are too big and complex to start with.</li>

</ul>

The input files for both testing the phonebook and the priority queues are generated randomly, based on certain rules. We have used a mix of names and surnames from a previous year’s class for the phonebook and created random phone numbers, e-mails and addresses. Please do not take any of the resulting names seriously.

<ul>

 <li></li>

</ul>