# THB1
package Bai3;

/**
 *
 * @author MSI-PC
 */
public class Main {
    public static void main(String[] args) {
        SinhVien[] dsSV = new SinhVien[3];
        dsSV[0] = new SinhVien("123", "Nguyễn Văn Vang");
        dsSV[1] = new SinhVien("543", "Nguyễn Thị Hà");
        dsSV[2] = new SinhVien("321", "Lương Văn lẹo");
         LopHocPhan lopHocPhan = new LopHocPhan("123", "LT Hướng đối tượng", "Nguyễn Văn Vang", "Thu 2, tiết 3-4, Phòng 201", dsSV);
            System.out.println("Mã LHP: " + lopHocPhan.getMaLHP());
        System.out.println("Tên LHP: " + lopHocPhan.getTenLHP());
        System.out.println("GV giảng dạy: " + lopHocPhan.getTenGV());
        System.out.println("Thông tin buổi hoc: " + lopHocPhan.getThongTinLopHoc());
        System.out.println("Danh sách sinh viên: ");
        for (SinhVien sv : lopHocPhan.getDsSV()) {
            System.out.println(sv.getMaSV() + "\t | " + sv.getHoTen());
            System.out.println("Tổng số sinh viên: " + lopHocPhan.getSoLuongSV());
    }
}

}
