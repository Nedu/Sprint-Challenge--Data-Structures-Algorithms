Add your answers to the Algorithms exercises here.

a) O(n)

b) O(log n)

c) O(log n * log n * log n)

d) O(n^2)

e) O(n^3 log n)

f) O(n)

g) O(n)

2a) 
const LRTA = (arr) => {
    let max = 0
    for(let i = 0; i < arr.length; i++) {
        for(let j = 0; j < arr.length; j++) {
            if (max < arr[j] - arr[i]) {
                max = arr[j] - arr[i];
            }
        }
    }
    return max
}

b) Start throwing eggs from the topmost floor of the building and record if the eggs break till you get to a floor where it doesn't break.

const f;
for(let i = building.length - 1; i <= 0; i--) {
    if(!eggBroken) {
        f = building[i];
        return f;
    }
}

3a) O(n^2) because we are going through each items and then sorting

b) O(nlogn) because since the pivot would always be a median we are cutting down running time.