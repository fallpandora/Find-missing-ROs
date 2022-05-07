# Find-missing-ROs
Using excel to find missing repair orders in a large PDF data set
-- This will assist any person that has to manages large sets of PDf's in the form of repair orders from dealer ships. 
-- When dealership apply for an increase for their warranty parts or labor departments. The dealerships have to review several hundred to even several thousand of pages to sequential repair orders to locate qualifying repair orders to send off to vehicle manufactuers to be approved. During this process many vehicle manufactuers request that your repairs order be sequential without any missing. Counting every repair order is a VERY time comsuming and ardious task.
With my developed process I have taken a task that would normally take 4 hours to accomplish down to just 5-10 mins.
--
[Finding missing for Reynolds.docx](https://github.com/fallpandora/Find-missing-ROs/files/8644462/Finding.missing.for.Reynolds.docx)
[Finding missing for ReynoldsPdf.pdf](https://github.com/fallpandora/Find-missing-ROs/files/8644475/Finding.missing.for.ReynoldsPdf.pdf)
--
The above folders are files explaining the complete process that I developed. 
--
The main formula you would want to use to read and find you missing is
SMALL(IF(COUNTIF($A$1:$A$721,ROW($719130:$719860))=0,ROW($719130:$719860),""),ROW(A1))
As you can see we changed five of the values
1. We made sure that we input the last cell number that contained the last RO (721).
2. We changed the value to the first RO (719130).
3. We changed the value to the last RO shown (719860). This process repeats for step 4 and 5.
4. (Again – 4. We changed the value to the first RO (719130). 5. We changed the value to the last RO shown
(719860).)
![image](https://user-images.githubusercontent.com/30642354/167238838-4c98c0c0-df98-45d3-bc6c-87f3d4d9da6d.png)
