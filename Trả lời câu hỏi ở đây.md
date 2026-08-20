Reflection Questions (after completing the exercise)
1.	Why must totalStudents be static instead of a regular instance field?
2.	Why must methods like FindTopStudent be static, while GetClassification() must not be?
3.	If you call student1.GetTotalStudents() (calling a static method through an object reference) — is this valid in C#? What happens, and does the compiler give any warning?
4.	What is the difference between accessing a static method via the class name (Student.GetTotalStudents()) and via an instance? Which one is considered good practice?

TRẢ LỜI

1.	Tại vì instnce field là một là một đối tượng mà student là một trong những lớp chứa đối tượng đó có các đối tượng nhỏ bên trong. Nên khi muốn đọc các đối tượng nhỏ trong đó thì phải có không gian chung to chứa các đối tượng đó để đọc xem có bao nhiêu. Nên dùng static
2.	Tương tự với câu 1, chúng ta cần có một không gian chung lớn để thực hiện.
3.	Lỗi cách gọi tên, phải gọi từ “to” đến “nhỏ” phải gọi qua class
4.	Gọi qua class tốt hơn, vì đó là cách đúng
