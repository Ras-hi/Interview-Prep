# Data Structures and Algorithms Code Templates

##  ✔️ Two pointers: one input, opposite ends

```javascript
function twoPointersOppositeEnds(arr) {
    let left = 0, right = arr.length - 1;
    while (left < right) {
        // Process elements arr[left] and arr[right]
        left++;
        right--;
    }
}


```

##  ✔️ Two pointers: two inputs, exhaust both

```javascript
function twoPointerstwoInputs(arr1, arr2) {
    int i=,j=0, ans =0;
    while(i<arr1.size() && j<arr2.size() ){
        if(condition meets) i++;
        else j++;
    }
    while(i<arr1.size()){
        //logic awaited
        i++;
    }
    while(j<arr2.size()){
        //logic awaited
        j++;
    }
    return ans;
}


```
##  ✔️ Sliding Window

```javascript
int fn(vector<int>& arr) {
    int left = 0, ans = 0, curr = 0;

    for (int right = 0; right < arr.size(); right++) {
        // do logic here to add arr[right] to curr

        while (WINDOW_CONDITION_BROKEN) {
            // remove arr[left] from curr
            left++;
        }

        // update ans
    }

    return ans;
}


```
##  ✔️ Building a prefix sum 

```javascript
vector<int> fn(vector<int>& arr) {
    vector<int> prefix(arr.size());
    prefix[0] = arr[0];

    for (int i = 1; i < arr.size(); i++) {
        prefix[i] = prefix[i - 1] + arr[i];
    }

    return prefix;
}


```
##  ✔️ Efficient string building

```javascript
string fn(vector<char>& arr) {
    return string(arr.begin(), arr.end())
}


```

##  ✔️ Linked list: fast and slow pointer

```javascript
int fn(ListNode* head) {
    ListNode* slow = head;
    ListNode* fast = head;
    int ans = 0;

    while (fast != nullptr && fast->next != nullptr) {
        // do logic
        slow = slow->next;
        fast = fast->next->next;
    }

    return ans;
}

```


##  ✔️ Reversing a Linked List

```javascript
Listnode* fn(Listnode* head) {
    Listnode* curr=head;
    Listnode* prev =nullptr;
    while(curr!=nullptr){
        Listnode* nextnode =curr->next;
        curr->next =prev;
        prev=curr;
        curr=nextnode;
    }
    return prev;
}


```


