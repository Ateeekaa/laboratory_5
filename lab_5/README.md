# Push – Navigator.push(context, MaterialPageRoute(builder: (context) => SecondScreen()));
→ FirstScreen-нен SecondScreen-ге өтеді, бірақ FirstScreen жабылмайды.
# PushNamed – Navigator.pushNamed(context, '/second');
→ Именованный маршрут арқылы SecondScreen-ге өтеді.
# PushReplacement – Navigator.pushReplacement(context, MaterialPageRoute(builder: (context) => SecondScreen()));
→ FirstScreen-ді SecondScreen-мен ауыстырады, бірақ артқа қайтуға болмайды.
# PushAndRemoveUntil – Navigator.pushAndRemoveUntil(context, MaterialPageRoute(builder: (context) => SecondScreen()), (route) => false);
→ Барлық алдыңғы экрандарды жауып, SecondScreen-ді ашады.
# PushNamedAndRemoveUntil – Navigator.pushAndRemoveUntil(context, '/second' as Route<Object?>, (route) => false);
→ Барлық экрандарды жауып, именованный маршрут арқылы SecondScreen-ді ашады.
# Pop – Navigator.pop(context);
→ Ағымдағы экранды жауып, алдыңғы экранға қайтарады.
# PopAndPushNamed – Navigator.popAndPushNamed(context, '/third');
→ Ағымдағы экранды жауып, орнына ThirdScreen ашады.