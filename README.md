# javaLinkedList
java 链表

##### 节点
```java
public class Node{
	Node next=null;
	int data;
	public Node(int data){
	   this.data=data;
	}
}

```
##### 构造链表类
```java
public class MyLinkdedList{
	
   Node head=null;
   // 添加节点
   private void addNode(int data){
       Node newNode=new Node(data);
       if(head==null){
          head=newNode;
          return;
       }
       Node temp=head;
       while(temp.next!=null){
            temp=temp.next;

       }
       temp.next=newNode;
   }


  // 链表的长度
  public int length(){
    int length=0;
    Node curNode=head;
    while(curNode!=null){
     length++;
      curNode=curNode.next;

    }
    return length;
  }
  
}

```
