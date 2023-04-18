# Day-01-Introduction-to-Browser-and-Web
Task 01 - Difference between HTTP 1.1 vs HTTP 2 and objects and its internal representation in Javascript

HTTP Stands for Hyper Text Transfer Protocol and it is used in client server communication

1. Difference between HTTP1.1 vs HTTP2
  
              HTTP 1.1                                            HTTP 2      
   *It works in textual format                          *It works on a Binary Protocol
   *The head of the line blocks all the request         *It allows multiplexing so on one TCP connection
   behind it until it doesnt get all its rsources        is required for multiple request
   *It compresses data by itself                        *It uses HPACK for data compression
   *All the information related to header file is       *The server sends all the other files like css & js 
   repeated in every request                             without the request using push frame
   *It can load one request at a time hence on          *It uses single TCP connection to deliver multiple 
   request per one TCP connection is possible            request
   *It reduces web traffic however there is an          *It pushes effectively and reduce the page load time
    increased risk of network congestion                 by greater margin 
   *This protocol introduces a warning header field     *It brings the fundamental semantics of HTTP 
    to carry additional information about the status      like headers
    of a message 
      
      
2. Objects and its internal representation in Javascript
                Objects in java script may be said as an unordered collection of related data in the form of
   "Key:Value" pairs.These keys can be variables or functions and are called properities and methods.Each objects may include 
   any mix of these fundamental data types and reference data types. The object storage location in memory is indicated by the 
   refrences or pointer.the values are not really kept in the variables.
   const school={
      name:'abc school'
      address:'street name'
      grade: 10
      }
      A property key may be a string and its value can be anything including text ,a number,an array, or even a function.
      there are two ways to access an objects property 
      *Dot Notation- ex. console.log(school.name)
      *Bracket Notation ex. console.log(school[name])  
