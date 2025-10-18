# TRIỀU VỸ SANDAL STORE - Website Bán Giày Sneaker

## Mô tả
Website bán giày sneaker cao cấp được xây dựng bằng Vue.js 3 với giao diện hiện đại. Dự án học tập tích hợp đầy đủ chức năng e-commerce cơ bản.

## Chức năng chính
- ✅ **Trang chủ**: Hiển thị sản phẩm nổi bật
- ✅ **Danh mục sản phẩm**: Nike, Vans, MLB, Gucci
- ✅ **Chi tiết sản phẩm**: Xem thông tin chi tiết giày
- ✅ **Giỏ hàng**: Thêm/xóa sản phẩm, tính tổng tiền
- ✅ **Tìm kiếm**: Tìm kiếm sản phẩm theo tên
- ✅ **Đăng ký/Đăng nhập**: Quản lý tài khoản người dùng
- ✅ **Hồ sơ cá nhân**: Xem và chỉnh sửa thông tin
- ✅ **Responsive**: Tương thích mobile và desktop

## Cấu trúc dự án

### Vue.js 3 Application
```
src/
├── App.vue                    # Root component
├── main.js                    # Entry point
├── eventBus.js                # Event bus cho communication
├── components/                # Vue components
│   ├── ComHeader.vue          # Header với navigation
│   ├── ComFooter.vue          # Footer
│   ├── ComHome.vue            # Trang chủ
│   ├── ComProduct.vue         # Hiển thị sản phẩm
│   ├── ComProductDetail.vue   # Chi tiết sản phẩm
│   ├── ComCart.vue            # Giỏ hàng
│   ├── ComTimKiem.vue         # Tìm kiếm
│   ├── ComNike.vue            # Danh mục Nike
│   ├── ComVans.vue            # Danh mục Vans
│   ├── ComMLB.vue             # Danh mục MLB
│   ├── ComGucci.vue           # Danh mục Gucci
│   ├── ComLogin.vue           # Đăng nhập
│   ├── ComRegister.vue        # Đăng ký
│   └── ComHoSo.vue            # Hồ sơ cá nhân
├── data/                      # Data management
│   ├── items.js               # Danh sách sản phẩm
│   ├── cart.js                # Giỏ hàng
│   └── users.js               # Tài khoản người dùng
└── router/
    └── index.js               # Vue Router configuration
```

## Công nghệ sử dụng
- **Vue.js 3** - Frontend framework
- **Vue Router 4** - Client-side routing
- **JavaScript ES6+** - Ngôn ngữ lập trình
- **CSS3** - Styling và responsive design
- **Event Bus** - Component communication
- **Local Storage** - Lưu trữ dữ liệu local

## Cài đặt

### 1. Yêu cầu
- Node.js 14+
- npm hoặc yarn
- Trình duyệt hiện đại

### 2. Cài đặt dependencies
```bash
npm install
```

### 3. Chạy development server
```bash
npm run serve
```
Truy cập: http://localhost:8080

### 4. Build cho production
```bash
npm run build
```

### 5. Lint code
```bash
npm run lint
```

## Cách sử dụng

### 1. Duyệt sản phẩm
- **Trang chủ**: Xem sản phẩm nổi bật
- **Sản phẩm**: Duyệt theo danh mục (Nike, Vans, MLB, Gucci)
- **Tìm kiếm**: Nhập tên sản phẩm vào ô tìm kiếm

### 2. Xem chi tiết sản phẩm
- Click vào sản phẩm để xem thông tin chi tiết
- Xem giá, mô tả, hình ảnh sản phẩm

### 3. Quản lý giỏ hàng
- **Thêm vào giỏ**: Click "Thêm vào giỏ hàng"
- **Xem giỏ hàng**: Click icon giỏ hàng ở header
- **Xóa sản phẩm**: Click "Xóa" trong giỏ hàng
- **Cập nhật số lượng**: Thay đổi số lượng sản phẩm

### 4. Tài khoản người dùng
- **Đăng ký**: Tạo tài khoản mới
- **Đăng nhập**: Đăng nhập với tài khoản có sẵn
- **Hồ sơ**: Xem và chỉnh sửa thông tin cá nhân

## Tính năng nổi bật

### 1. Responsive Design
- Tương thích với mọi kích thước màn hình
- Mobile-first approach
- Navigation menu responsive

### 2. Component Architecture
- Tách biệt logic và UI
- Reusable components
- Props và events communication

### 3. State Management
- Event Bus cho global state
- Local Storage persistence
- Reactive data binding

### 4. Routing
- Single Page Application (SPA)
- Dynamic routing với parameters
- Navigation guards

### 5. Search Functionality
- Real-time search
- Search across all products
- Case-insensitive search

## Cấu trúc dữ liệu

### Sản phẩm (items.js)
```javascript
{
  id: Number,
  name: String,
  image: String,
  description: String,
  price: Number,
  quality: Number
}
```

### Giỏ hàng (cart.js)
```javascript
{
  id: Number,
  name: String,
  price: Number,
  quantity: Number,
  image: String
}
```

## Lưu ý
- Đây là dự án học tập Vue.js 3
- Dữ liệu được lưu trong localStorage
- Không có backend server
- Phù hợp để học Vue.js và e-commerce frontend
