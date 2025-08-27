let marks = [45, 67, 89, 23, 99, 76];

function findMaxFor(marks) {
  let max = marks[0];
  for (let i = 1; i < marks.length; i++) {
    if (marks[i] > max) {
      max = marks[i];
    }
  }
  return max;
}

function findMaxWhile(marks) {
  let i = 0;
  let max = marks[0];
  while (i < marks.length) {
    if (marks[i] > max) {
      max = marks[i];
    }
    i++;
  }
  return max;
}

function findMaxForEach(marks) {
  let max = marks[0];
  marks.forEach(function(mark) {
    if (mark > max) {
      max = mark;
    }
  });
  return max;
}

// ----------------- Run All -----------------
console.log("Marks:", marks);
console.log("Highest (for):", findMaxFor(marks));
console.log("Highest (while):", findMaxWhile(marks));
console.log("Highest (forEach):", findMaxForEach(marks));
