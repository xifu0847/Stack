# Stack
#include <iostream>
#include <stack>
#include <vector>

using namespace std;

int main(){
    //declare a stack
    stack<int> st;
    vector<int> v{2,3,4,5};
    //{1,3,4,5,6}
    st.push(1);
    //cout << st.size() << endl;
    st.pop();
    //cout << st.size() << endl;
    st.push(3);
    //cout << st.top() << endl;
    st.push(4);
    st.push(5);
    //cout << st.size() << endl;
    st.pop();
    //cout << st.size() << endl;
    
    for(int i =0; i<v.size(); i++){
        st.push(v[i]);
    }
    //cout << st.size() << endl;
    //cout << st.top() << endl;
    
    /*for(int i = 0; i<st.size(); i++){ 
        cout << st.top() << endl;
        st.pop(); 
    }
    */ //stack size在变化
    
    while(st.size() > 0){
        cout << st.top() << endl;
        st.pop();
    }
    // st.empty() if st.size() == 0 return true else return false
    
    //https://leetcode.com/problems/backspace-string-compare/
    //https://leetcode.com/problems/valid-parentheses/
    //https://leetcode.com/problems/trapping-rain-water/
    
    //S =abc##
    //T= a
}
