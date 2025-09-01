# qr_generator.py
import qrcode

def make_qr():
    text = input("🔗 متن یا لینک خود را وارد کنید: ")
    img = qrcode.make(text)
    img.save("qrcode.png")
    print("✅ کد QR ساخته شد و در فایل qrcode.png ذخیره شد.")

if __name__ == "__main__":
    make_qr()
