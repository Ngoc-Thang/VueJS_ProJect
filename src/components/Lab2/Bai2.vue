<template>


<div class="container mt-3">
  <h3>Bài tập ứng dụng Modal cho Tài khoản</h3>

  <button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#myModal">
    Tài khoản
  </button>
</div>

<!-- The Modal -->
<div class="modal" id="myModal">
  <div class="modal-dialog">
    <div class="modal-content">

      <div class="modal-header">
        <h4 class="modal-title">ĐĂNG NHẬP/ ĐĂNG KÝ</h4>
        <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
      </div>

      <div class="modal-body">
        <!-- Add your content here -->
         

    <div class="container mt-4">
        <ul class="nav nav-tabs" id="myTab" role="tablist">
            <!-- Tab Headers -->
            <li class="nav-item" role="presentation">
                <button 
                    class="nav-link active" 
                    id="register-tab" 
                    data-bs-toggle="tab" 
                    data-bs-target="#register" 
                    type="button" 
                    role="tab" 
                    aria-controls="register" 
                    aria-selected="true">
                    Đăng Ký
                </button>
            </li>
            <li class="nav-item" role="presentation">
                <button 
                    class="nav-link" 
                    id="login-tab" 
                    data-bs-toggle="tab" 
                    data-bs-target="#login" 
                    type="button" 
                    role="tab" 
                    aria-controls="login" 
                    aria-selected="false">
                    Đăng Nhập
                </button>
            </li>
        </ul>

        <div class="tab-content mt-4" id="myTabContent">
            <!-- Registration Form -->
            <div class="tab-pane fade show active" id="register" role="tabpanel" aria-labelledby="register-tab">
                <div class="card p-4">
                    <h5 class="card-title">Form Đăng Ký Thông Tin</h5>
                    <form>
                        <div class="mb-3">
                            <label for="fullName" class="form-label">Họ và Tên</label>
                            <input type="text" class="form-control" id="fullName" placeholder="Nhập họ và tên">
                        </div>
                        <div class="mb-3">
                            <label for="email" class="form-label">Email</label>
                            <input type="email" class="form-control" id="email" placeholder="Nhập email">
                        </div>
                        <div class="mb-3">
                            <label for="phone" class="form-label">Số Điện Thoại</label>
                            <input type="text" class="form-control" id="phone" placeholder="Nhập số điện thoại">
                        </div>
                        <div class="mb-3">
                            <label for="password" class="form-label">Mật Khẩu</label>
                            <input type="password" class="form-control" id="password" placeholder="Nhập mật khẩu">
                        </div>
                        <div class="mb-3">
                            <label for="confirmPassword" class="form-label">Xác Nhận Mật Khẩu</label>
                            <input type="password" class="form-control" id="confirmPassword" placeholder="Xác nhận mật khẩu">
                        </div>
                        <div class="mb-3">
                            <label class="form-label">Giới Tính</label>
                            <div>
                                <div class="form-check form-check-inline">
                                    <input class="form-check-input" type="radio" name="gender" id="male" value="Nam">
                                    <label class="form-check-label" for="male">Nam</label>
                                </div>
                                <div class="form-check form-check-inline">
                                    <input class="form-check-input" type="radio" name="gender" id="female" value="Nữ">
                                    <label class="form-check-label" for="female">Nữ</label>
                                </div>
                            </div>
                        </div>
                        <div class="mb-3">
                            <label for="language" class="form-label">Ngôn Ngữ</label>
                            <select class="form-select" id="language">
                                <option selected>Tiếng Việt</option>
                                <option>English</option>
                            </select>
                        </div>
                        <div class="mb-3 form-check">
                            <input type="checkbox" class="form-check-input" id="agreeTerms">
                            <label class="form-check-label" for="agreeTerms">Tôi đồng ý với các điều khoản và điều kiện</label>
                        </div>
                        <button type="submit" class="btn btn-primary">Đăng Ký</button>
                    </form>
                </div>
            </div>

            <!-- Login Form -->
            <div class="tab-pane fade" id="login" role="tabpanel" aria-labelledby="login-tab">
                <div class="card p-4">
                    <h5 class="card-title">Form Đăng nhập</h5>
                    <form>
                        <div class="mb-3">
                            <label for="loginEmail" class="form-label">Email</label>
                            <input type="email" class="form-control" id="loginEmail" placeholder="Nhập email">
                        </div>
                        <div class="mb-3">
                            <label for="loginPassword" class="form-label">Mật Khẩu</label>
                            <input type="password" class="form-control" id="loginPassword" placeholder="Nhập mật khẩu">
                        </div>
                        <button type="submit" class="btn btn-primary">Đăng Nhập</button>
                    </form>
                </div>
            </div>
        </div>
    </div>
      </div>

    </div>
  </div>
</div>




</template>

<script>
export default {
  name: "Lab2Bai2",
};
</script>

<!-- Bootstrap JS (for tab functionality) -->
