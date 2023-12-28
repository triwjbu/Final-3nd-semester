# Phân biệt các phạm vi try cập private, public, protected, default trong java: 


| Mức Độ Truy Cập | Cùng Lớp | Cùng Package | Lớp Con (Subclass) | Bất Kỳ Nơi Nào |
|------------------|----------|--------------|--------------------|----------------|
| `public`         | ✓        | ✓            | ✓                  | ✓              |
| `protected`      | ✓        | ✓            | ✓                  | ✗              |
| `default`        | ✓        | ✓            | ✗                  | ✗              |
| `private`        | ✓        | ✗            | ✗                  | ✗              |

# cho biết ý nghĩa và mục đích của các hàm get/set trong một lớp
1. **Hàm Get (Getter):**
   - **Ý Nghĩa:** Hàm get được sử dụng để đọc giá trị của một thuộc tính từ bên ngoài lớp.
   - **Mục Đích:** Cung cấp một cách an toàn để truy cập giá trị của thuộc tính private từ bên ngoài lớp mà không cần trực tiếp truy cập vào thuộc tính đó.


2. **Hàm Set (Setter):**
   - **Ý Nghĩa:** Hàm set được sử dụng để gán giá trị cho một thuộc tính từ bên ngoài lớp.
   - **Mục Đích:** Cung cấp một cách an toàn để thay đổi giá trị của thuộc tính private từ bên ngoài lớp mà không cần trực tiếp gán giá trị đó.


3. **Mục Đích Chung:**
   - Bảo vệ tính toàn vẹn của dữ liệu: Bằng cách sử dụng getter và setter, lớp có thể kiểm soát cách giá trị của thuộc tính được đọc và ghi.
   - Đối tượng hóa quy ước: Việc sử dụng getter và setter giúp đảm bảo rằng các thay đổi trong cách dữ liệu được lưu trữ không ảnh hưởng đến mã nguồn bên ngoài lớp.
   - Phản ánh (Reflection): Hàm get/set cũng hữu ích khi làm việc với phản ánh, cho phép bạn thao tác với thuộc tính của một đối tượng trong thời gian chạy.

# Lớp là gì? Đối tượng là gì? Phân biệt lớp và đối tượng

## Khái niệm
1. **Lớp (Class):**
	
	- Lớp là một mô hình, một khuôn mẫu (blueprint) để tạo ra các đối tượng.
	- Nó định nghĩa các thuộc tính (dữ liệu) và phương thức (hành vi) mà mỗi đối tượng của lớp sẽ có.
	- Lớp không phải là một đối tượng cụ thể, mà là một khuôn mẫu chung để tạo ra các đối tượng.
2. **Đối tượng (Object):**
	
	- Đối tượng là một thực thể cụ thể được tạo ra từ một lớp cụ thể.
	- Nó biểu diễn một cá thể cụ thể của một lớp, với các thuộc tính cụ thể và có thể thực hiện các hành động cụ thể.
	- Đối tượng có thể được xem như là một thể hiện (instance) của một lớp.

## **Phân biệt:**

- **Lớp (Class):**
	
	- Là một mô hình chung, khuôn mẫu cho việc tạo ra các đối tượng.
	- Định nghĩa thuộc tính và phương thức mà các đối tượng sẽ có.
	- Không phải là một đối tượng cụ thể.
	- Ví dụ: Lớp "Hình tròn" có thể có thuộc tính bán kính và phương thức tính diện tích.
- **Đối tượng (Object):**
	
	- Là một thực thể cụ thể được tạo ra từ lớp.
	- Có các thuộc tính và hành vi cụ thể dựa trên định nghĩa của lớp.
	- Là một thể hiện của một lớp.
	- Ví dụ: Một đối tượng cụ thể của lớp "Hình tròn" có thể có bán kính là 5 và có thể tính diện tích.
# Lớp cơ sở trừu tượng là gì?

Lớp cơ sở trừu tượng (abstract base class) là một loại lớp mà không thể tạo ra đối tượng cụ thể từ nó. Nó thường chứa các phương thức trừu tượng (abstract methods), những phương thức mà chỉ có định nghĩa, không có cài đặt cụ thể. Lớp cơ sở trừu tượng thường được sử dụng để định nghĩa giao diện chung cho các lớp con.
# Trình bày các đặc điểm quan trọng của LTHĐT.

## **Đa hình (Polymorphism):**
- **Đa hình tại thời điểm biên dịch và chạy:** Đa hình cho phép một đối tượng có thể thay đổi hành vi của nó dựa trên lớp mà nó thuộc về. Đa hình cung cấp tính linh hoạt và tái sử dụng mã nguồn.
## **Kế thừa (Inheritance):**
- **Chia sẻ và mở rộng:** Kế thừa cho phép một lớp con kế thừa thuộc tính và phương thức từ một lớp cha, giúp tái sử dụng mã nguồn và tạo ra các lớp có quan hệ chung.
## **Đóng gói (Encapsulation):**
- **Bảo vệ dữ liệu:** Đóng gói giữ cho dữ liệu (trong các trường) và hành vi (trong các phương thức) của một đối tượng được bảo vệ và không thể truy cập trực tiếp từ bên ngoài.
## **Abstract và Interface:**
- **Lớp trừu tượng và giao diện:** Lập trình hướng đối tượng hỗ trợ các khái niệm như lớp trừu tượng và giao diện, giúp định nghĩa các hợp đồng và định nghĩa chung cho các lớp con.
# Lập trình hướng đối tượng là gì?

Lập trình hướng đối tượng là phương pháp lập trình lấy đối tượng làm nền tảng để xây dựng thuật giải xây dựng chương trình

# Nêu khái niệm Constructor, Destructor. Phân biệt Constructor mặc định và Contructor khác. Phân biệt Constructor và Destructor.

## Khái niệm 

**Constructor:**

- **Khái niệm:** Constructor là một phương thức đặc biệt trong lập trình hướng đối tượng được sử dụng để khởi tạo một đối tượng khi nó được tạo ra từ một lớp. Constructor thường chứa các câu lệnh để thiết lập giá trị ban đầu cho các thuộc tính của đối tượng.

**Destructor:**

- **Khái niệm:** Destructor là một phương thức khác được sử dụng để giải phóng tài nguyên (bộ nhớ, tài nguyên hệ thống, v.v.) mà một đối tượng đã chiếm giữ trước khi nó bị hủy. Destructor thường được sử dụng để làm sạch sau khi đối tượng không còn cần thiết nữa.
## Phân biệt 
**Constructor mặc định và Constructor khác:**

- **Constructor mặc định:** Là một constructor không có tham số. Nếu một lớp không có bất kỳ constructor nào, Java sẽ tạo ra một constructor mặc định tự động cho lớp đó.
- **Constructor khác:** Là constructor có tham số. Nó được gọi khi một đối tượng được tạo ra và cần truyền các giá trị cụ thể để khởi tạo đối tượng.

**Constructor và Destructor:**

- **Constructor:** Được gọi khi một đối tượng được tạo ra và sử dụng để khởi tạo giá trị ban đầu.
- **Destructor:** Được gọi khi một đối tượng sắp bị hủy và sử dụng để giải phóng tài nguyên.

**Phân biệt chính:**

1. **Chức năng:**
    
    - **Constructor:** Khởi tạo giá trị ban đầu cho đối tượng.
    - **Destructor:** Giải phóng tài nguyên khi đối tượng bị hủy.
2. **Gọi khi nào:**
    
    - **Constructor:** Được gọi khi đối tượng được tạo ra.
    - **Destructor:** Được gọi khi đối tượng sắp bị hủy.
3. **Cú pháp:**
    
    - **Constructor:** Cùng tên với lớp, không có kiểu trả về, có thể có hoặc không có tham số.
    - **Destructor:** Cùng tên với lớp, có tiền tố `~`, không có tham số và không có giá trị trả về.
#   Nêu khái niệm về sự kế thừa và những ưu điểm và nhược điểm của kế thừa trong LTHDT

## Khái niệm 

 **Kế thừa** trong lập trình hướng đối tượng là một khái niệm quan trọng, cho phép một lớp (lớp con) kế thừa thuộc tính và phương thức từ một lớp khác (lớp cha). Kế thừa giúp tái sử dụng mã nguồn, mở rộng chức năng của lớp và xây dựng các mức trừu tượng khác nhau.

## Ưu điểm 

1. **Tái sử dụng mã nguồn (Code Reusability):** Kế thừa cho phép lớp con sử dụng lại mã nguồn của lớp cha, giúp giảm việc viết lại mã và tăng khả năng tái sử dụng.

2. **Mở rộng chức năng (Functionality Extension):** Lớp con có thể mở rộng hoặc sửa đổi chức năng của lớp cha bằng cách thêm các phương thức mới hoặc ghi đè (override) các phương thức đã có.

3. **Tính trừu tượng (Abstraction):** Kế thừa cung cấp khả năng tạo ra các lớp trừu tượng, giúp mô hình hóa các mối quan hệ và chức năng chung.

4. **Quản lý mã nguồn (Code Management):** Khi có thay đổi ở một lớp cha, tất cả các lớp con kế thừa từ nó cũng sẽ được ảnh hưởng. Điều này giúp quản lý mã nguồn hiệu quả hơn.

## Nhược điểm 

1. **Rủi ro thiếu rõ ràng (Ambiguity):** Khi một lớp con kế thừa từ nhiều lớp cha hoặc lớp cha có nhiều phương thức trùng tên, có thể gây ra rủi ro thiếu rõ ràng và hiểu lầm.

2. **Giao tiếp chặt chẽ (Tight Coupling):** Sự chia sẻ mã nguồn có thể tạo ra sự kết nối chặt chẽ giữa lớp cha và lớp con, làm giảm tính linh hoạt và tái sử dụng.

3. **Vấn đề dư thừa (Redundancy):** Kế thừa có thể dẫn đến vấn đề dư thừa khi lớp con kế thừa các phương thức hoặc thuộc tính không cần thiết từ lớp cha.

4. **Khả năng hiểu lầm và lạc quan hệ (Misunderstandings and Misuse):** Kế thừa không đúng cách có thể dẫn đến hiểu lầm và lạc quan hệ, làm giảm tính linh hoạt của mã nguồn.
#  Phân biệt khái niệm overload và override trong LTHDT

## Overload (Nạp chồng)
 
1. **Khái niệm:** Overload là quá trình định nghĩa nhiều hàm hoặc phương thức có cùng tên trong một lớp hoặc một gói (namespace), nhưng khác nhau về số lượng hoặc kiểu dữ liệu của các tham số.
  
2. **Tính chất:**
   - Overload không yêu cầu mối quan hệ kế thừa giữa các hàm.
   - Các hàm được overload phải có cùng tên nhưng có tham số khác nhau.

3. **Được thực hiện:** Tại thời điểm biên dịch.

4. **Ví dụ (Java):**
   ```java
   class MathOperations {
       int add(int a, int b) {
           return a + b;
       }

       double add(double a, double b) {
           return a + b;
       }
   }
   ```

## Override (Ghi đè)
1. **Khái niệm:** Override là quá trình triển khai lại (hoặc định nghĩa lại) một phương thức đã được định nghĩa trong lớp cha trong lớp con. Phương thức ở lớp con phải có cùng tên, kiểu trả về và tham số như phương thức ở lớp cha.

2. **Tính chất:**
   - Override yêu cầu có mối quan hệ kế thừa giữa lớp cha và lớp con.
   - Các phương thức được override phải có cùng tên, kiểu trả về và tham số.

3. **Được thực hiện:** Tại thời điểm chạy (runtime).

4. **Ví dụ (Java):**
   ```java
   class Animal {
       void makeSound() {
           System.out.println("Animal makes a sound");
       }
   }

   class Dog extends Animal {
       @Override
       void makeSound() {
           System.out.println("Dog barks");
       }
   }
   ```

**Tóm tắt:**
- **Overload:** Định nghĩa nhiều hàm có cùng tên nhưng khác nhau về tham số trong một lớp hoặc gói.
- **Override:** Triển khai lại một phương thức của lớp cha trong lớp con, giữ nguyên tên, kiểu trả về và tham số. Yêu cầu mối quan hệ kế thừa giữa lớp cha và lớp con.

# Trình bày khái niệm đa hình trong LTHĐT

**Đa hình** trong lập trình hướng đối tượng (OOP) là một khái niệm quan trọng, cho phép một đối tượng có thể thay đổi hành vi của nó dựa trên lớp mà nó thuộc về. Đa hình có hai dạng: đa hình compile-time (compile-time polymorphism) và đa hình runtime (runtime polymorphism).

## **Đa hình compile-time (Overloading):**
   - **Khái niệm:** Đa hình tại thời điểm biên dịch xảy ra khi một lớp có nhiều phương thức cùng tên nhưng khác nhau về số lượng hoặc kiểu dữ liệu của tham số.
   - **Cơ chế:** Compiler sẽ quyết định cụ thể phương thức nào sẽ được gọi dựa trên thông tin đã biết tại thời điểm biên dịch.
   - **Ví dụ (Java):**
     ```java
     class MathOperations {
         int add(int a, int b) {
             return a + b;
         }

         double add(double a, double b) {
             return a + b;
         }
     }
     ```

## **Đa hình runtime (Override):**
   - **Khái niệm:** Đa hình tại thời điểm chạy xảy ra khi một lớp con kế thừa từ một lớp cha và triển khai lại (override) một hoặc nhiều phương thức của lớp cha.
   - **Cơ chế:** Khi gọi một phương thức trên một đối tượng, chương trình sẽ tùy thuộc vào loại đối tượng để quyết định phương thức cụ thể nào sẽ được gọi.
   - **Ví dụ (Java):**
     ```java
     class Animal {
         void makeSound() {
             System.out.println("Animal makes a sound");
         }
     }

     class Dog extends Animal {
         @Override
         void makeSound() {
             System.out.println("Dog barks");
         }
     }
     ```

**Tính chất chung của Đa hình:**
- **Tính linh hoạt (Flexibility):** Đa hình giúp mã nguồn trở nên linh hoạt, cho phép thay đổi hành vi của đối tượng mà không làm thay đổi cấu trúc của mã nguồn.

- **Tính mở rộng (Extensibility):** Đa hình cho phép thêm mới hoặc mở rộng chức năng của chương trình mà không cần sửa đổi mã nguồn hiện tại.
# Tài liệu tham khảo

https://www.studocu.com/vn/document/truong-dai-hoc-cong-nghe-thong-tin-dai-hoc-quoc-gia-thanh-pho-ho-chi-minh/nhap-mon-lap-trinh/ly-thuyet-oop-da-tong-hop/54305649