
# Môn: Phát triển ứng dụng trên thiết bị dữ liệu
# Họ tên : Nguyễn Đình Tú
# MSSV: K225480106067
# Lớp : K58KTP

# BÀI LÀM

# Bài 1 Viết phần mềm trên công cụ Mit App inventor

BƯỚC 1: Tạo Project

Vào trang:

  https://ai2.appinventor.mit.edu

Bấm:

  Create Apps

Đăng nhập Gmail.

<img width="691" height="372" alt="image" src="https://github.com/user-attachments/assets/745502ff-54cf-40d4-96ce-51501e3ce0dd" />

Sau đó bấm:

  Projects → Start new project

Đặt tên:

  App_GioiThieu_GiaiToan_WebView

<img width="692" height="390" alt="image" src="https://github.com/user-attachments/assets/7f786a3f-ca2d-416c-a6c8-f9fe0457cf17" />

Bấm OK.

<img width="691" height="389" alt="image" src="https://github.com/user-attachments/assets/d0a27997-c9dc-4fc2-9335-b73ee7ac9eb7" />

BƯỚC 2: Tạo đủ 3 Screen

Mặc định đã có:
	
  Screen1

<img width="691" height="349" alt="image" src="https://github.com/user-attachments/assets/8088a5f0-702a-4905-8a90-a9bfc2d61e73" />

Tạo thêm Screen2:

	Add Screen → Screen2 → OK

<img width="692" height="356" alt="image" src="https://github.com/user-attachments/assets/575e1eed-61cc-4546-bc48-5d40f3b625e0" />

Tạo thêm Screen3:

	Add Screen → Screen3 → OK

<img width="691" height="345" alt="image" src="https://github.com/user-attachments/assets/656612e8-3575-495d-84f6-11e1f1a4f303" />

Kiểm tra góc trên có danh sách:
  	Screen1
	  
    Screen2
	  
    Screen3
    
<img width="692" height="281" alt="image" src="https://github.com/user-attachments/assets/19aa7d53-46c5-44a4-a4ea-1f65f7643530" />

# PHẦN A: SCREEN1 — ABOUT

BƯỚC 3: Thiết kế Screen1

Chọn Screen1.

Ở bên phải Properties, sửa:

  Title: About
	
  AlignHorizontal: Center
	
  AlignVertical: Center
	
  Scrollable: true
	
  BackgroundColor: tùy chọn


BƯỚC 4: Kéo Label tiêu đề

Tại cửa sổ Designer, trong vùng Palette chọn nhóm User Interface, sau đó kéo thành phần Label vào vùng Viewer (mô phỏng màn hình điện thoại).

Thao tác kéo thả này giúp tạo nhanh giao diện mà không cần viết mã nguồn. Sau khi kéo Label vào màn hình, thành phần sẽ xuất hiện trong khu vực Components, đồng thời các thuộc tính của Label sẽ hiển thị trong khu vực Properties để người dùng chỉnh sửa.

Bên trái Palette → User Interface.

Kéo:

  Label

vào màn hình điện thoại.

Chọn Label đó, sửa Properties:

  Text: THÔNG TIN CÁ NHÂN
	
  FontSize: 22
	
  FontBold: true
	
  TextAlignment: Center
	
  Width: Fill parent

<img width="691" height="358" alt="image" src="https://github.com/user-attachments/assets/579d3783-70a3-447d-b77d-f5f9237b93a1" />

Ý nghĩa:


  Text: thay đổi nội dung hiển thị.

  FontSize: tăng kích thước chữ.

  FontBold: hiển thị chữ đậm.

  TextAlignment: căn giữa nội dung.

  Width = Fill Parent: giúp Label chiếm toàn bộ chiều ngang màn hình.

BƯỚC 6: Kéo Button sang Screen2

trong Palette → User Interface, kéo thành phần Button vào màn hình.

Sau khi kéo vào, Button xuất hiện trong danh sách Components. Tại đây đổi tên Button thành:

  btnGiaiToan

Việc đổi tên giúp dễ nhận biết và thuận lợi khi lập trình Block sau này.

Tiếp tục thay đổi thuộc tính:

Text: Giải bài toán đơn giản

Thuộc tính Text quyết định nội dung hiển thị trên nút bấm.

Kéo:

  Button

Đổi tên ở phần Components:

  btnGiaiToan

Sửa Text:

  Giải bài toán đơn giản

<img width="691" height="334" alt="image" src="https://github.com/user-attachments/assets/0402afe4-ab73-4687-9174-57f21b5075ee" />

BƯỚC 7: Kéo Button sang Screen3

Kéo thêm:

  Button

<img width="691" height="348" alt="image" src="https://github.com/user-attachments/assets/14424f8e-2c80-4ba4-b3ec-1a18f1c0bcf7" />

Đổi tên:

	btnWebView

<img width="691" height="348" alt="image" src="https://github.com/user-attachments/assets/4c507c20-cefa-44c9-bf27-8d92c49777a8" />

Sửa Text:

	Mở trang web

<img width="692" height="344" alt="image" src="https://github.com/user-attachments/assets/b39df133-8c62-45eb-8c13-6cd3e02978b3" />

BƯỚC 8: Blocks cho Screen1

Chuyển từ tab Designer sang tab Blocks.

Tại đây App Inventor sử dụng phương pháp lập trình trực quan bằng cách kéo và ghép các khối lệnh thay vì viết code bằng Java hoặc Kotlin.

Bấm tab:

  Blocks

<img width="691" height="377" alt="image" src="https://github.com/user-attachments/assets/6456c556-ede4-46e4-837c-9c89772873c5" />

Tạo block 1:
	
  when btnGiaiToan.Click
	
  do open another screen screenName "Screen2"

Cách kéo:

btnGiaiToan → when btnGiaiToan.Click

Control → open another screen screenName

Text → "Screen2"

<img width="692" height="333" alt="image" src="https://github.com/user-attachments/assets/cb191fbb-f222-4d32-aad5-1430a413cfe4" />

Ý nghĩa:

Khi người dùng nhấn nút Giải bài toán đơn giản, ứng dụng sẽ tự động chuyển sang màn hình Screen2.

Ưu điểm của lập trình bằng Block:

Không cần nhớ cú pháp.

Hạn chế lỗi lập trình.

Dễ quan sát luồng xử lý.

Nhược điểm:

Khi ứng dụng lớn sẽ có rất nhiều Block.

Khó quản lý hơn mã nguồn chuyên nghiệp.

<img width="692" height="333" alt="image" src="https://github.com/user-attachments/assets/2b5f521e-c466-4cd5-8722-4e955d1975c9" />

Tạo block 2:

when btnWebView.Click

do open another screen screenName "Screen3"

Cách kéo:

btnWebView → when btnWebView.Click

Control → open another screen screenName

Text → "Screen3"

<img width="691" height="368" alt="image" src="https://github.com/user-attachments/assets/fab67c58-40f2-4467-86c2-01d54320d711" />

# PHẦN B: SCREEN2 — TÍNH TỔNG HAI SỐ

BƯỚC 9: Chọn Screen2

Góc trên chọn:

  Screen2

<img width="691" height="343" alt="image" src="https://github.com/user-attachments/assets/fca65294-23c8-4fdb-9060-decde2232ef4" />

Sửa Properties:

	Title: Giải toán
  
	AlignHorizontal: Center
	
  AlignVertical: Center
	
  Scrollable: true

<img width="691" height="351" alt="image" src="https://github.com/user-attachments/assets/1739d69c-75f7-4bac-8675-64c91fdc19fd" />

BƯỚC 10: Kéo Label tiêu đề Screen2

Kéo:

  Label

<img width="691" height="343" alt="image" src="https://github.com/user-attachments/assets/dda3711d-2fbb-49ab-b4fd-5a41c1756b87" />

Sửa:

  Text: TÍNH TỔNG HAI SỐ
	
  FontSize: 22
	
  FontBold: true
	
  Width: Fill parent
	
  TextAlignment: Center

<img width="692" height="331" alt="image" src="https://github.com/user-attachments/assets/a509f10d-ce59-42f2-90dd-8e5e6b3486ea" />

BƯỚC 11: Kéo TextBox số thứ nhất

Kéo:

  TextBox

Đổi tên:

  txtSoA

<img width="691" height="346" alt="image" src="https://github.com/user-attachments/assets/027e70d1-6bb8-4d4d-8eb2-bfea148713b1" />

Sửa:

  Hint: Nhập số thứ nhất
	
  NumbersOnly: true
	
  Width: Fill parent

<img width="692" height="365" alt="image" src="https://github.com/user-attachments/assets/a6e0c799-17a2-4a90-8917-96a6d73088e0" />

BƯỚC 12: Kéo TextBox số thứ hai

Kéo thêm:

  TextBox

<img width="692" height="322" alt="image" src="https://github.com/user-attachments/assets/3705cc29-bd70-49f1-a6c2-15e3e98b5c19" />

Đổi tên:

	txtSoB

Sửa:

  Hint: Nhập số thứ hai
	
  NumbersOnly: true
	
  Width: Fill parent

<img width="691" height="311" alt="image" src="https://github.com/user-attachments/assets/63db09f6-afc6-4aea-9264-d56711908969" />

BƯỚC 13: Kéo Button tính tổng

Kéo:

  Button

Đổi tên:

  btnTinh

<img width="692" height="357" alt="image" src="https://github.com/user-attachments/assets/b790b3f2-4c58-4a16-8f67-92876edcd200" />

Sửa Text:

	Tính tổng

<img width="692" height="333" alt="image" src="https://github.com/user-attachments/assets/e5c5f4ea-031f-42a9-8313-94465e213655" />

BƯỚC 14: Kéo Label kết quả

Kéo:

  Label

<img width="692" height="323" alt="image" src="https://github.com/user-attachments/assets/32045c43-be42-46a3-ba69-1dc45e796beb" />

Đổi tên:

	lblKetQua

<img width="692" height="295" alt="image" src="https://github.com/user-attachments/assets/e5ed2093-722a-4328-a71d-8226c16f04c4" />

Sửa Text:

	Kết quả:

<img width="691" height="345" alt="image" src="https://github.com/user-attachments/assets/f16a735c-43df-429e-babc-fe632e542223" />

BƯỚC 15: Kéo Button quay lại

Kéo:

	Button

<img width="691" height="347" alt="image" src="https://github.com/user-attachments/assets/004e77d7-187b-405c-8ba5-bad7affa484f" />

Đổi tên:

	btnBack1

<img width="691" height="345" alt="image" src="https://github.com/user-attachments/assets/892186d5-e98a-4571-b156-0faf7cd419a1" />

Sửa Text:

	Quay lại

<img width="691" height="373" alt="image" src="https://github.com/user-attachments/assets/0e11423a-f4e3-4cb4-9318-939f7ab5f71b" />

BƯỚC 16: Blocks cho Screen2

Bấm Blocks.

Block tính tổng:

  do set lblKetQua.Text to join "Kết quả: " (txtSoA.Text + 	txtSoB.Text)

Cách kéo:

  btnTinh → when btnTinh.Click
	
  lblKetQua → set lblKetQua.Text to
	
  Text → join
	
  Text → "Kết quả: "
	
  Math → +
	
  txtSoA → txtSoA.Text
	
  txtSoB → txtSoB.Text

<img width="691" height="374" alt="image" src="https://github.com/user-attachments/assets/15c80d75-055b-43f1-84bd-554cdc32ebab" />

Block quay lại:

	when btnBack1.Click

  do close screen

Cách kéo:

  btnBack1 → when btnBack1.Click
	
  Control → close screen

# PHẦN C: SCREEN3 — WEBVIEW

BƯỚC 17: Chọn Screen3

Góc trên chọn:

	Screen3

Sửa Properties:

  Title: WebView
	
  AlignHorizontal: Center
	
  AlignVertical: Center
	
  Scrollable: false

<img width="692" height="365" alt="image" src="https://github.com/user-attachments/assets/9a09ae83-1acc-432d-bc76-5f3919f6983b" />

BƯỚC 18: Kéo Label tiêu đề

Kéo:

  Label

Sửa:

  Text: HIỂN THỊ TRANG WEB
	
  FontSize: 20
	
  FontBold: true
	
  Width: Fill parent
	
  TextAlignment: Center

<img width="691" height="359" alt="image" src="https://github.com/user-attachments/assets/828a5c78-3a2c-4819-9ae1-29ed8307a1a2" />

BƯỚC 19: Kéo WebViewer

Trong Palette → User Interface, kéo:

WebViewer

Đổi tên:

  WebViewer1

Sửa:

  Width: Fill parent
	
  Height: Fill parent
	
  HomeUrl: https://www.tnut.edu.vn

<img width="691" height="367" alt="image" src="https://github.com/user-attachments/assets/e6b7ed4c-aa81-453e-8537-caac2b890fed" />

BƯỚC 20: Kéo Button quay lại

Kéo:

  Button

<img width="691" height="340" alt="image" src="https://github.com/user-attachments/assets/df1b9290-eeb6-4a61-a5b7-4899612871c6" />

Đổi tên:

	btnBack2

<img width="692" height="331" alt="image" src="https://github.com/user-attachments/assets/6b6c6834-98fe-4dd4-82cc-ba5584c30929" />

Sửa Text:
	
  Quay lại

<img width="692" height="315" alt="image" src="https://github.com/user-attachments/assets/eed59013-ffa2-44a0-8fa7-79fdb0ad72c3" />

BƯỚC 21: Blocks cho Screen3

Bấm Blocks.

Block mở web:

  when Screen3.Initialize
	
  do call WebViewer1.GoToUrl url "https://www.tnut.edu.vn"

<img width="691" height="356" alt="image" src="https://github.com/user-attachments/assets/c370c09d-1a28-4f4e-8409-d06c2cb2de9f" />

Cách kéo:

  Screen3 → when Screen3.Initialize
	
  WebViewer1 → call WebViewer1.GoToUrl
	
  Text → "https://www.tnut.edu.vn"

<img width="691" height="265" alt="image" src="https://github.com/user-attachments/assets/5e30da51-30a0-4741-b64a-38c237a07e0c" />

Block quay lại:


  when btnBack2.Click
	
  do close screen

Cách kéo:

  btnBack2 → when btnBack2.Click
	
  Control → close screen

<img width="692" height="335" alt="image" src="https://github.com/user-attachments/assets/55e4d3c0-69ce-4e40-995e-897b28d55e66" />

* Kết quả cuối cùng đạt được 

1 abuot ( giới thiệu bản thân)

<img width="519" height="442" alt="image" src="https://github.com/user-attachments/assets/25cb0361-c07e-4549-a9ea-b855b13e0bbb" />

2 Giai bài toán 

<img width="633" height="488" alt="image" src="https://github.com/user-attachments/assets/a086cf58-9a9c-4a65-92a0-a7d7d6ae4858" />

3 web view 

<img width="466" height="624" alt="image" src="https://github.com/user-attachments/assets/2f527401-ff13-4d8d-8a8f-eab289b0b86d" />

# Bài 2: BÀI TẬP ANDROID STUDIO

# A. PHẦN LÝ THUYẾT

1. AndroidManifest.xml

AndroidManifest.xml là file khai báo cấu hình chính của ứng dụng Android.

File này dùng để mô tả:

- Tên ứng dụng.

- Package của ứng dụng.

- Các Activity có trong app.

- Activity nào chạy đầu tiên.

- App cần quyền gì.

- Theme, icon, label của app.

- App có sử dụng Internet, camera, bộ nhớ, vị trí hay không.

Ví dụ khai báo quyền Internet:

<uses-permission android:name="android.permission.INTERNET" />

* Ý nghĩa:

- Cho phép app truy cập Internet.

- Dùng để gọi API.

- Dùng để mở WebView.

- Nếu không khai báo quyền này, app có thể không gửi được dữ liệu lên server.

Ví dụ khai báo Activity:

<activity android:name=".MainActivity" />

<activity android:name=".SolveActivity" />

<activity android:name=".WebActivity" />

Activity chạy đầu tiên được khai báo như sau:

<intent-filter>

  <action android:name="android.intent.action.MAIN" />
  
    <category android:name="android.intent.category.LAUNCHER" />
    
</intent-filter>

2. Vòng đời của một ứng dụng Android

Một Activity trong Android có vòng đời gồm các hàm chính:

onCreate()

onStart()

onResume()

onPause()

onStop()

onRestart()

onDestroy()

* Ý nghĩa:

- onCreate(): Activity được tạo lần đầu.

- onStart(): Activity bắt đầu hiển thị.

- onResume(): Người dùng có thể tương tác với màn hình.

- onPause(): Activity tạm dừng.

- onStop(): Activity không còn hiển thị.

- onRestart(): Activity được mở lại.

- onDestroy(): Activity bị hủy.

Khi tạo project Android Studio, code tự sinh có sẵn hàm:

@Override

protected void onCreate(Bundle savedInstanceState) {

    super.onCreate(savedInstanceState);
    
    setContentView(R.layout.activity_main);

}

* Lý do có onCreate():

- Đây là hàm đầu tiên được gọi khi Activity được tạo.

- Dùng để gắn giao diện XML vào Java.

- Dùng để ánh xạ Button, TextView, EditText.

- Dùng để viết code khởi tạo ban đầu.

3. Kiểm tra quyền trong app

Một số quyền phải kiểm tra khi app đang chạy, ví dụ Camera, Location.

Ví dụ code kiểm tra quyền:

if (checkSelfPermission(Manifest.permission.CAMERA)

        != PackageManager.PERMISSION_GRANTED) {
    
    requestPermissions(new String[]{Manifest.permission.CAMERA}, 100);

}

* Ý nghĩa:

- checkSelfPermission: kiểm tra app đã có quyền chưa.

- requestPermissions: xin quyền từ người dùng.

- 100: mã request để xử lý kết quả trả về.

Với quyền Internet, chỉ cần khai báo trong Manifest:

<uses-permission android:name="android.permission.INTERNET" />

4. Giao diện Android trong res/layout

Giao diện Android thường được mô tả bằng file XML trong thư mục:

res/layout

* Ví dụ:

activity_main.xml

activity_solve.xml

activity_web.xml

Các đối tượng giao diện thường dùng:

- TextView: hiển thị văn bản.

- EditText: nhập dữ liệu.

- Button: nút bấm.

- WebView: hiển thị trang web.

- LinearLayout: chứa và sắp xếp các đối tượng con.

5. Tránh hardcode trong XML

Không nên viết trực tiếp:

  android:text="Giải toán"

Nên lưu trong file:

res/values/strings.xml

* Ví dụ:

<string name="btn_solve">Mở màn hình giải toán</string>

Sau đó tham chiếu trong layout:

android:text="@string/btn_solve"

Cú pháp tham chiếu:

@string/tên_chuỗi

@color/tên_màu

@drawable/tên_ảnh

@style/tên_style

* Ưu điểm:

- Dễ sửa nội dung.

- Tránh lặp lại.

- Dễ dịch sang nhiều ngôn ngữ.

- Hỗ trợ theme sáng/tối.

- Android tự chọn tài nguyên phù hợp theo ngôn ngữ, vị trí, theme của người dùng.

Ví dụ:

res/values/strings.xml        → tiếng Việt mặc định

res/values-en/strings.xml     → tiếng Anh

res/values-night/colors.xml   → màu cho chế độ tối

Nhờ cơ chế này, app có thể tự hiển thị đúng ngôn ngữ và giao diện phù hợp với người dùng.

6. Đối tượng chứa trong layout

LinearLayout dùng để chứa các đối tượng con.

Sắp xếp theo chiều dọc:

android:orientation="vertical"

Sắp xếp theo chiều ngang:

android:orientation="horizontal"

Căn giữa các đối tượng con:

android:gravity="center"

Ví dụ:

<LinearLayout

  android:orientation="vertical"
  
    android:gravity="center">

</LinearLayout>

7. Code tương tác với layout

Để Java tương tác với layout, cần dùng id.

Trong XML:

<TextView

  android:id="@+id/txtResult"
  
    android:layout_width="match_parent"
    
    android:layout_height="wrap_content" />

Trong Java:

TextView txtResult = findViewById(R.id.txtResult);

txtResult.setText(getString(R.string.app_name));

Muốn text phù hợp với ngôn ngữ, vị trí, theme thì không hardcode:

Không nên:

txtResult.setText("Kết quả");

Nên dùng:

txtResult.setText(getString(R.string.result_text));

8. Sự kiện người dùng

* Sự kiện là hành động người dùng tác động vào app, ví dụ:

- Click Button.

- Click TextView.

- Nhập dữ liệu.

 -Chọn item.

Có 2 cách xử lý sự kiện click.

Cách 1: Viết trong Java bằng setOnClickListener

Button btn = findViewById(R.id.btnSolve);

btn.setOnClickListener(v -> {

    txtResult.setText("Đã bấm nút");
    
});

Cách 2: Khai báo trong XML bằng android:onClick

Trong XML:

<Button

  android:onClick="xuLyClick" />

Trong Java:

public void xuLyClick(View view) {

    txtResult.setText("Đã bấm nút");

}

9. Thư mục Assets

Assets là thư mục đặc biệt trong Android.

Đường dẫn:

app/src/main/assets

Khi copy file vào thư mục này, các file sẽ được đóng gói theo app khi biên dịch.

App có thể truy cập file trong Assets bằng cú pháp:

InputStream is = getAssets().open("ten_file.json");

Lợi ích:

- App có sẵn dữ liệu.

- Dùng được khi không có Internet.

- Phù hợp với app hướng dẫn, app học tập, app từ điển, app xem tài liệu offline.

* Ứng dụng:

- App hướng dẫn học Android offline.

- App đọc danh sách bài học từ file JSON.

- App hiển thị nội dung bằng TextView hoặc RecyclerView.

# B. PHẦN THỰC HÀNH

APP1: App_HuongDanAndroid_Offline

* Giao diện trang Android Studio

<img width="691" height="389" alt="image" src="https://github.com/user-attachments/assets/7817ceb4-c9c5-49c1-aa17-3ad68e99ebe6" />

1. Tạo project APP1

Mở Android Studio → chọn:

New Project → Empty Views Activity

<img width="691" height="389" alt="image" src="https://github.com/user-attachments/assets/5f5abfe3-b8de-4142-82dd-fa4081b3b3c0" />

Điền:

Name: 	App_HuongDanAndroid_Offline

Language: Java

Minimum SDK: API 23 hoặc cao hơn

<img width="691" height="389" alt="image" src="https://github.com/user-attachments/assets/bbd60ad7-d120-4a88-aaf9-2441cb3578a1" />

Bấm Finish.

2. Tạo thư mục Assets

Trong Android Studio, nhìn bên trái chọn chế độ Project.

Đi theo đường dẫn:

app/src/main

Chuột phải vào main → New → Directory → đặt tên:

Assets

<img width="692" height="384" alt="image" src="https://github.com/user-attachments/assets/2c4273ad-80d7-44d3-800c-a112a5202f7b" />

Kết quả:

app/src/main/assets

3. Tạo file lessons.json

Chuột phải vào thư mục assets → New → File → đặt tên:

lessons.json

<img width="692" height="382" alt="image" src="https://github.com/user-attachments/assets/8637e886-c7c9-42c5-9246-f4d333ea640f" />

Dán nội dung này:

<img width="692" height="384" alt="image" src="https://github.com/user-attachments/assets/1587f690-a593-48e4-a6af-6b64a16c602b" />

4. Sửa giao diện activity_main.xml

Mở file:

  app/src/main/res/layout/activity_main.xml

<img width="691" height="389" alt="image" src="https://github.com/user-attachments/assets/e4d90a25-afb4-4398-92be-faa452abb4eb" />

Xóa hết nội dung cũ, dán code này:	

<img width="691" height="389" alt="image" src="https://github.com/user-attachments/assets/04db22ba-ea60-4efa-85fb-5b5f1686771d" />

5. Sửa MainActivity.java

Mở file:

  app/src/main/java/.../MainActivity.java

Dán code này:

<img width="691" height="389" alt="image" src="https://github.com/user-attachments/assets/dc07a2e4-35ab-4994-95c1-7c9dbafacb86" />

6. Chạy APP1
   
* Kết quả đạt được

<img width="691" height="389" alt="image" src="https://github.com/user-attachments/assets/4e9ec3c8-92bf-492f-8931-455c59fcaea8" />

APP2: App_GiaiToan_WebView

1. Tạo project APP2

Android Studio → New Project → Empty Views Activity

<img width="691" height="389" alt="image" src="https://github.com/user-attachments/assets/37c6ed5f-d206-46e8-824e-f1b899d432fe" />

Điền:

Name: App_GiaiToan_WebView

Language: Java

Minimum SDK: API 23 hoặc cao hơn

<img width="691" height="389" alt="image" src="https://github.com/user-attachments/assets/69fe7995-f1ad-4ddf-aa17-0447f313c745" />

Bấm Finish.

2. Tạo 3 Activity

App cần 3 màn hình:

MainActivity.java   → màn hình About

SolveActivity.java  → màn hình Giải toán

WebActivity.java    → màn hình WebView

<img width="692" height="390" alt="image" src="https://github.com/user-attachments/assets/021ebc40-0291-4527-bc5f-6a304a0e66e0" />

3. Tạo SolveActivity

Chuột phải vào package Java:

app/java/com.example.app_giaitoan_webview

Chọn:

New → Activity → Empty Views Activity

Đặt tên:

SolveActivity

<img width="692" height="394" alt="image" src="https://github.com/user-attachments/assets/d7286658-e442-4685-9995-a3ddd0a59638" />

Bấm Finish.

4. Tạo WebActivity

Làm tương tự:

New → Activity → Empty Views Activity

Đặt tên:

WebActivity

<img width="691" height="397" alt="image" src="https://github.com/user-attachments/assets/4119aefe-19e9-4dc7-9f6f-6313d0c97fff" />

Bấm Finish.

5. Sửa AndroidManifest.xml

Mở:

  app/src/main/AndroidManifest.xml

<img width="666" height="250" alt="image" src="https://github.com/user-attachments/assets/0be5b233-49ae-43ad-8e40-898127c31d96" />

Sửa thành:

<img width="692" height="397" alt="image" src="https://github.com/user-attachments/assets/ba923f5a-da12-44ad-a749-b594611d650b" />

6. Sửa strings.xml

Mở:

  app/src/main/res/values/strings.xml

<img width="692" height="374" alt="image" src="https://github.com/user-attachments/assets/eddfa5d3-d8a3-4312-9806-a70260c0dbed" />

Dán:

<img width="691" height="399" alt="image" src="https://github.com/user-attachments/assets/fe01598a-01d0-4878-8897-e0b8674388b6" />

7. Giao diện Activity 1: About

Mở:

  res/layout/activity_main.xml


<img width="692" height="384" alt="image" src="https://github.com/user-attachments/assets/c1986400-7d86-4092-93c4-7dcbdc7cdc87" />

Dán:

<img width="692" height="259" alt="image" src="https://github.com/user-attachments/assets/9c0b1984-9a0b-4954-91dc-e78f53027dde" />

8. Code MainActivity.java

Mở MainActivity.java 
  
<img width="691" height="396" alt="image" src="https://github.com/user-attachments/assets/81e812db-4321-4d44-83d5-4ab211616832" />

9. Giao diện Activity 2: Giải toán

Mở:

  res/layout/activity_solve.xml

<img width="692" height="399" alt="image" src="https://github.com/user-attachments/assets/a5a888c5-6a47-4fc6-a98a-9c78dd4d2f2e" />

Dán:

10. Code SolveActivity.java

<img width="692" height="329" alt="image" src="https://github.com/user-attachments/assets/954da063-3d2c-4851-b59c-f66aa96bafa5" />

Mở SolveActivity.java :

<img width="691" height="399" alt="image" src="https://github.com/user-attachments/assets/728d2074-c221-43c7-8ece-64226c5b0686" />

11. Giao diện Activity 3: WebView

Mở:

  res/layout/activity_web.xml

<img width="692" height="385" alt="image" src="https://github.com/user-attachments/assets/406a6dc2-8d12-434c-9104-30a5c6ac9151" />

Dán:

<img width="693" height="532" alt="image" src="https://github.com/user-attachments/assets/31eb4a55-927f-4a16-8ac8-7bd0443a320c" />

12. Code WebActivity.java

Mở WebActivity.java :

<img width="692" height="579" alt="image" src="https://github.com/user-attachments/assets/5ac080f0-a635-463d-9115-739c347d1223" />

13. Chạy thử APP2

Thứ tự test:

1. Chạy app

2. Màn hình About hiện ra

<img width="692" height="635" alt="image" src="https://github.com/user-attachments/assets/d0f2eb11-f4d3-4080-a575-a253a2b93be1" />

3. Bấm “Mở màn hình giải toán”

<img width="693" height="730" alt="image" src="https://github.com/user-attachments/assets/54e78429-f12a-40f3-b957-b85bfdc9eb48" />

4. Nhập a = 1, b = 2

5. Bấm “Giải và gửi API”

6. App hiển thị nghiệm x = -2

![Uploading image.png…]()

8. Quay lại

![Uploading image.png…]()

9. Bấm “Mở trang WebView”

10. Trang https://k58kmt.tdh.io.vn?masv=K225480106067 hiển thị

![Uploading image.png…]()

