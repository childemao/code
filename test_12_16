// 将一个字符串中所有的空格替换为 %20
//
#include <iostream>
#include <string>

class Solution {
public:
    void replaceSpace(char *str,int length) {
        int countOfBlank = 0;
        int lenOfOriginalStr = 0;
        char * p = str;
        if(str == NULL)
        {
            return;
        }

        while(*p)
        {
            ++lenOfOriginalStr;
            if(*p++ == ' ')
            {
                ++countOfBlank;
            }
        }

        int len_total = lenOfOriginalStr + 2 * countOfBlank;
        char * str1 = str + len_total; // 指针偏移到 '\0'
        char * str2 = str + lenOfOriginalStr; // 指针偏移到原始字符串最后

        while(str1 > str2)
        {
            if(*str2 == ' ')
            {
                *str1-- = '0';
                *str1-- = '2';
                *str1 = '%';
            }
            else
            {
                *str1 = *str2;
            }

            --str1;
            --str2;
        }


    }

};
