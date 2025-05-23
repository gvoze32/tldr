# find

> البحث عن الملفات أو المُجَلَّدات داخل فروع مُجَلَّد، بشكل متكرر.
> لمزيد من التفاصيل: <https://manned.org/find>.

- البحث عن الملفات حسب الامتداد:

`find {{root_path}} -name '{{*.ext}}'`

- البحث عن الملفات المطابقة لأنماط مسار/اسم متعددة:

`find {{root_path}} -path '{{*/path/*/*.ext}}' -or -name '{{*pattern*}}'`

- البحث عن المُجَلَّدات المطابقة لاسم معين، مع تجاهل حالة الأحرف سواء أكانت صغيرة او كبيرة:

`find {{root_path}} -type d -iname '{{*lib*}}'`

- البحث عن الملفات المطابقة لنمط معين، مع استثناء مسارات محددة:

`find {{root_path}} -name '{{*.py}}' -not -path '{{*/site-packages/*}}'`

- البحث عن الملفات التي تطابق نطاق حجم معين، مع تقييد العمق التكراري إلى "1":

`find {{root_path}} -maxdepth 1 -size {{+500k}} -size {{-10M}}`

- تنفيذ أمر لكل ملف (استخدم `{}` داخل الأمر للوصول إلى اسم الملف):

`find {{root_path}} -name '{{*.ext}}' -exec {{wc -l}} {} \;`

- البحث عن جميع الملفات المعدلة اليوم وتمرير النتائج إلى أمر واحد كوسيطات:

`find {{root_path}} -daystart -mtime {{-1}} -exec {{tar -cvf archive.tar}} {} \+`

- البحث عن الملفات أو المُجَلَّدات الفارغة وحذفها مع عرض التفاصيل:

`find {{root_path}} -type {{f|d}} -empty -delete -print`
