import java.util.Scanner;

public class NotificationSettings {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        // وضعیت اولیه اعلان‌ها فعال است (true)
        boolean isNotificationsActive = true;

        while (true) {
            System.out.println("\n--- منوی تنظیمات اعلان‌ها ---");
            System.out.println("1. فعال‌کردن اعلان‌ها");
            System.out.println("2. غیرفعال‌کردن اعلان‌ها");
            System.out.println("3. مشاهده وضعیت اعلان‌ها");
            System.out.println("4. بازگرداندن تنظیمات پیش‌فرض");
            System.out.println("5. خروج از برنامه");
            System.out.print("لطفاً شماره گزینه موردنظر را وارد کنید: ");

            // بررسی اینکه آیا ورودی عدد است یا خیر
            if (!scanner.hasNextInt()) {
                System.out.println("گزینه نامعتبر است.");
                scanner.next(); // پاک کردن ورودی نامعتبر از اسکنر
                continue;
            }

            int choice = scanner.nextInt();

            // استفاده از ساختار switch-case برای مدیریت انتخاب‌های کاربر
            switch (choice) {
                case 1:
                    isNotificationsActive = true;
                    System.out.println("✅ اعلان‌ها با موفقیت فعال شدند.");
                    break;
                
                case 2:
                    isNotificationsActive = false;
                    System.out.println("🔕 اعلان‌ها غیرفعال شدند.");
                    break;
                
                case 3:
                    if (isNotificationsActive) {
                        System.out.println("ℹ️ وضعیت فعلی اعلان‌ها: فعال");
                    } else {
                        System.out.println("ℹ️ وضعیت فعلی اعلان‌ها: غیرفعال");
                    }
                    break;
                
                case 4:
                    isNotificationsActive = true; // پیش‌فرض فعال است
                    System.out.println("🔄 تنظیمات به حالت پیش‌فرض بازگردانده شد (اعلان‌ها فعال هستند).");
                    break;
                
                case 5:
                    System.out.println("خروج از برنامه. روز خوش!");
                    scanner.close();
                    return; // پایان اجرای برنامه
                
                default:
                    // اگر عددی خارج از محدوده ۱ تا ۵ وارد شود
                    System.out.println("گزینه نامعتبر است.");
                    break;
            }
        }
    }
}
