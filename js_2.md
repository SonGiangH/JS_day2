* 3 từ khoá để khai báo biến trong Javascript :
    1. Let là từ khoá local, chỉ có tác dụng trong 1 khối block code.
    2. var là từ khoá global, có tác dụng trong toàn bộ chương trình, tuỳ theo nhu cầu sử dụng mà có thể dùng var hay let (vì liên quan đến dung lượng bộ nhớ khi xử lý)
    3. const là từ khoá để khai báo biến hằng số.

    ## Nguyên tắc đặt tên biến:

    1. Tuân theo nguyên tắc camelCase.
    2. Phân biệt chữ hoa chữ thường (Case sensitive).
    3. Không đặt tên biến trùng với từ khoá của Javascript.
    4. Đặt tên biến có nghĩa.
    5. Tên biến bắt đầu với : chữ cái, dấu $ , dấu _
    6. Hằng số luôn viết UPPERCASE

    > Primitive types of variables (Kiểu dữ liệu nguyên thuỷ của biến)
        1. String (chuỗi)
        2. Number (số)
        3. Boolean  (logic)
        4. undefined
        5. null

    ## Object 
    1. Đối tượng là một kiểu dữ liệu, cho lưu trữ nhiều kiểu dữ liệu cũng như giá trị khác nhau trong 1 biến duy nhất.

        * ví dụ: let presidentAmerica = {
            name: "Barrack Obama",
            age : 49,
            address: {
                street: "Humrey",
                city: "Chicago",
                state: "Illinois",
            }
            relationship: "single"
        }

    ## Function

    * function là cách thức tổ chức mã cơ bản trong JavaScript, function được sử dụng để đóng gói một
        đoạn mã để xử lý một công việc/tính toán giá trị nào đó, cho phép tái sử dụng đoạn mã ở nhiều nơi
        trong chương trình.

    * ví dụ: function functionName() {
    }

    * Function có thể trả về kết quả nhất định hoặc chỉ thực hiện chức năng tính toán trả về kiểu undefined.
    * Function có thể có tham số hoặc không có tham số truyền vào.
    * Gọi function chỉ cần gọi tên function trong code.   

    ***
    horizonal rules                 


    ## Logic 

*	Javascript tự ghép kiểu không giống như các ngôn ngữ khác
*	Có 2 qui tắc trong ép kiểu trong Javascript:
    1.	Với phép cộng : nếu 1 trong 2 phần tử có kiểu chuỗi (string) thì giá trị còn lại cũng chuyển sang kiểu chuỗi.
    2.	Các toán tử khác (-,*,/): ưu tiên chuyển sang số.

    ***
    horizonal rules
 
 
*	String rỗng, 0, null, undefined, NaN : chuyển về Boolean là false. Còn lại là true.
 
*	Increment and decrement: có 2 cách viết (let a = 1)
    1.	a++, a—(post fix) : tính trước tăng sau. let result = 10 + a++; // tính ra kết quả 11, xong a mới ++ thành 2
    2.	++a, --a( pre-fix) : tăng trước tính sau. let result = 10 + ++a; // a tăng trước (a=2) , rồi mới tính ra kết quả 10 + 2 = 12 
 

*	Equal ( ==, !=) : tự động chuyển đổi kiểu dữ liệu
*	Strict equal (===): không tự động chuyển đổi kiểu dữ liệu, so sánh nghiêm ngặt.
*	Các toán tử ++,--, ==, != , ===, !== 
*	Toán tử so sánh : so sánh các kí tự thì nó so sánh vị trí của kí tự trong bảng mã unicode. So sánh kí tự từ trái sang phải, không quan tâm độ dài chuỗi hay các kí tự phía sau 
    (“Be” > “Bazzzzzzzzzzzzzz”) so sánh từng kí tự 
*	Kí tự “ “ trống có giá trị trong bảng Unicode
*	Mọi biểu thức so sánh với NaN đều cho kết quả là false kể cả
    so sánh với chính nó.

    ***
    horizonal rules


    ## Chuyển đổi logic trong Javascript

*	NOT (!) chuyển đổi kiểu logic và đảo ngược ( !0 = true, !”0” = false, !null = true,…)
*	AND (&&) đánh giá toán hạm hoặc biểu thức thành giá trị logic (đúng sai) , trả về kết quả đầu tiên là false, nếu không có toán hạng nào là false thì trả về thằng cuối cùng.
    “Thầy giáo đẹp trai” && 0 && (1+2) ->  trả về 0 (chuỗi đầu tiên true -> skip, đến 0 là false thì nó trả về luôn)
    “Thầy giáo đẹp trai” && (1+2) && 1 -> trả về 1 ( vì không thằng nào false nên trả về thằng cuối cùng là 1 )
*	OR ( ||) hoặc :  đánh giá toán hạng biểu thức thành giá trị logic rồi trả về kết quả đầu tiên là true, nếu không có thằng nào là true thì trả về thằng cuối cùng.

 
    
    ### Some examples

Let a = 1;
Let b = 22;
Let name = ‘John’;
	b + a = 23
	c -> undefined
	a+name = 1John
	a+name+b = 1John22
	a+b+name= 122John
	name + a = John1
	name + b = John22
	name + (a + b) = John23
	`Hello ${name}` = Hello John
`${name}+1` = John1
`${name+1}` = John1
`${name}+a` = Johna
`a + b = ${a+b}` => “a + b =23”
`a +b = ${1+2}` => “ a + b = 3”
