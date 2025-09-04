
ANALYSIS ANSWERS:

 Q1. Explained Variance in PCA  
PCA puts parts in order based on how much they show changes in the data.  
When you look at a chart of these changes, the first few parts show most of it.  
In the Wine dataset, the first 2 or 3 parts usually show about 95% of the total change.  
This means you can go from 13 details to just 2 or 3 and still keep most of the useful info.


 Q2. PCA vs. LDA  
PCA is a method that works without knowing the group names. It tries to keep the biggest changes in the data.  
LDA is a method that uses group names and tries to make the groups easy to tell apart.  
PCA may keep changes that don’t help with sorting things.  
LDA focuses only on what helps split the groups clearly.  
So, LDA often gives better results when you want to sort or label things.


 Q3. KPCA and Gamma  
Gamma (γ) is a number that controls how much each point affects the shape in KPCA.  
If γ is too small (like 0.01), the shape is too smooth and groups mix together.  
If γ is too big (like 100), the shape is too sharp and may fit noise, not real patterns.  
A middle value (like γ = 15) often works best, making the groups easy to split.



 Q4. Classifier Performance  
Using the original data can be slow and sometimes less correct, because it has too many details.  
PCA makes the data smaller and faster to use, but may lose some group info.  
LDA also makes the data smaller, but keeps the group differences strong, so it often works better than PCA.  
For sorting tasks, LDA is usually better.  
PCA is great when you just want to shrink the data or show it in pictures.



Q5. Limits and Fixes  
PCA doesn’t work well with twisty or round shapes like circles or moons.  
It only sees straight-line changes.  
KPCA fixes this by using a trick to move the data into a new space.  
In that space, round shapes can be split easily.  
So, KPCA is better for tricky shapes that PCA can’t handle.


