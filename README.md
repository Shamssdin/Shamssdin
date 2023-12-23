import random

class PlasticInjectionProcess:
    def __init__(self, material, mold_temperature):
        self.material = material
        self.mold_temperature = mold_temperature

    def inject_plastic(self, pressure):
        # محاكاة عملية حقن البلاستيك
        print(f"جاري حقن المواد البلاستيكية بضغط {pressure} بار...")
        # يمكن إضافة المزيد من الخوارزميات والمحاكاة حسب الحاجة
        return True

    def monitor_quality(self):
        # محاكاة رصد جودة المنتج
        quality_score = random.uniform(0.8, 1.0)
        print(f"تم رصد جودة المنتج بنسبة {quality_score * 100}%.")

# تكوين العملية
plastic_process = PlasticInjectionProcess("ABS", 180)

# محاكاة دورة حقن البلاستيك
for _ in range(5):
    injection_pressure = random.randint(100, 200)
    if plastic_process.inject_plastic(injection_pressure):
        plastic_process.monitor_quality()
    print("\n")
    
