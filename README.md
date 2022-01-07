# ki_baglacinin_yazimi_deep_learningg
 "Ki" nin bağlaç mı ek mi olduğunun tespiti
 
 
Sequence Tagging Modeli kullanarak bir cümledeki "ki" nin bağlaç mı yoksa ek mi olduğuna karar veriyoruz.
Öncelikle cümlelerimiz hatalı "ki"leri taglıyoruz.

İnput Sentence: Toksöz ailesinin sahipliğinde ki Sağra çalışanlarının sendikası Genel İşten şikayetler aldık
Label Sentence: O O E O O O O O O O

Sonra Modelimizi eğitiyoruz


SONUÇLAR:

Score: 1855 in 2000 sentences

Orginal: herkesin kendi içerisinde büyük planları var tabii ki isterim

Wrong: herkesin kendi içerisinde büyük planları var tabiiki isterim

Prediction: herkesin kendi içerisinde büyük planları var tabii ki isterim


              precision    recall  f1-score   support

          E        0.98      0.93      0.96      2168
          O        0.95      0.93      0.94      3588
