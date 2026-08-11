# Chỉnh sửa Timeoff Request

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person   | A,M,D | Change Description | Version |
| -------------- | --------------- | ----- | ------------------ | ------- |
| Jul 16, 2026   | Nguyễn Duy Hiếu | A     |                    | 1.0.0   |

## I. Giới Thiệu Chung

{% hint style="info" %}
**Dành cho:** Admin CX

**Đường dẫn:** [https://ops.sapp.edu.vn/](https://ops.sapp.edu.vn/)
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Chấm công Giảng viên (Teacher Attendance) – Attendance Adjustment
* **Chức năng chính:** Chỉnh sửa và hủy phiếu Timeoff Request loại Attendance Adjustment
* **Module liên quan:**
  * Timeoff Request
  * Teacher (Quản lý giảng viên)
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết

* User đã đăng nhập thành công vào hệ thống OPS.
* User có quyền chỉnh sửa/hủy Timeoff Request.
* Phiếu cần thao tác có **Request Type = Attendance Adjustment** và **Status = Pending**.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Action của Timeoff Request theo trạng thái</summary>

Tại màn danh sách/chi tiết Timeoff Request loại Attendance Adjustment, khi User click **Action**, hệ thống hiển thị action theo trạng thái:

| Status    | View | Edit  | Cancel |
| --------- | ---- | ----- | ------ |
| Pending   | Có   | Có    | Có     |
| Approved  | Có   | Không | Không  |
| Rejected  | Có   | Không | Không  |
| Cancelled | Có   | Không | Không  |

> **Lưu ý:** Edit/Cancel chỉ áp dụng với request trạng thái **Pending**. Với request **Approved/Rejected**, hệ thống không cho sửa/hủy để đảm bảo lịch sử phê duyệt và dữ liệu Attendance Tracking không bị thay đổi ngoài luồng.

</details>

<details>

<summary>Chỉnh sửa Timeoff Request</summary>

> 🎯 _Mục tiêu: Cập nhật thông tin phiếu Attendance Adjustment đang ở trạng thái Pending._

{% stepper %}
{% step %}
**Truy cập màn danh sách Timeoff Request / Attendance Adjustment**
{% endstep %}

{% step %}
**Chọn request cần chỉnh sửa**
{% endstep %}

{% step %}
**Click "Action" → "Edit"**

Hệ thống mở màn Edit Request, các thông tin hiển thị mặc định theo dữ liệu request đang lưu.

<figure><img src="../../.gitbook/assets/image (1437).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Cập nhật thông tin request**

* **Các trường được phép chỉnh sửa:** Request Name, Reason, Upload Evidence, Check-in, Check-out.
* **Các trường không cho chỉnh sửa:** Request Type, Teacher Name, Class Code, Timeoff Date, Approver.
{% endstep %}

{% step %}
**Click "Save"**

Hệ thống validate thông tin. Nếu hợp lệ: cập nhật dữ liệu request, giữ nguyên **Status = Pending**, cập nhật Date/Updated at, gửi message **"Update successfully"**.
{% endstep %}
{% endstepper %}

{% hint style="info" %}
ℹ️ **Email cập nhật:** Sau khi chỉnh sửa thành công, hệ thống gửi mail thông báo cập nhật request đến Approver tương ứng — Title: _Thông báo request đã được cập nhật: `[Tên request]`_.
{% endhint %}

</details>

<details>

<summary>Hủy Timeoff Request</summary>

> 🎯 _Mục tiêu: Hủy phiếu Attendance Adjustment đang ở trạng thái Pending._

{% stepper %}
{% step %}
**Truy cập màn danh sách Timeoff Request / Attendance Adjustment**
{% endstep %}

{% step %}
**Chọn request cần hủy**
{% endstep %}

{% step %}
**Click "Action" → "Cancel"**

Hệ thống hiển thị confirmation popup: _"Are you sure to Cancel this Request?"_
{% endstep %}

{% step %}
**Xác nhận hủy request**

* Chọn **No:** hệ thống đóng popup, quay lại màn Timeoff Request, request không thay đổi.
* Chọn **Yes:** hệ thống hủy request, cập nhật **Status = Cancelled**, hiển thị message **"Cancel successfully"**.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Chỉ được **Edit/Cancel** phiếu ở trạng thái **Pending**.
2. Phiếu **Approved/Rejected** không cho phép Edit/Cancel để bảo toàn lịch sử phê duyệt và dữ liệu Attendance Tracking.
3. Khi Edit, các trường Request Type, Teacher Name, Class Code, Timeoff Date, Approver **không được thay đổi**.
4. Sau khi Edit, trạng thái phiếu **giữ nguyên Pending** và hệ thống gửi mail cập nhật cho Approver.
5. Việc Edit phiếu Pending **chưa** cập nhật Attendance Tracking (vì phiếu chưa được approve); Cancel phiếu Pending **không** cập nhật Attendance Tracking.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Nếu phát hiện phiếu Pending bị sai, hãy Edit trực tiếp thay vì tạo phiếu mới (tránh trùng phiếu).
2. Rà soát lại Check-in/Check-out và bằng chứng trước khi Save để Approver duyệt nhanh hơn.
{% endhint %}

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                   | Nguyên nhân                                         | Cách xử lý                                                                     |
| ---------------------------------- | --------------------------------------------------- | ------------------------------------------------------------------------------ |
| Không thấy action Edit/Cancel      | Phiếu đang ở trạng thái Approved/Rejected/Cancelled | Chỉ phiếu Pending mới có Edit/Cancel; các trạng thái khác chỉ có View          |
| Không Save được khi Edit           | Chưa nhập đủ/đúng các trường Required               | Kiểm tra Request Name, Reason, Evidence, Check-in/Check-out theo rule validate |
| Chỉnh sửa nhưng công chưa thay đổi | Phiếu vẫn ở trạng thái Pending, chưa được approve   | Attendance Tracking chỉ cập nhật sau khi phiếu được Approved                   |
