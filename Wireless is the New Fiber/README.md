A new type of unbounded-bandwidth wireless communication has just been tested and proved to be a suitable replacement for the existing, fiber-based communications network, which is struggling to keep up with traffic growth.

نوع جدیدی از ارتباط بی سیم پهنای باند-نامحدود به تازگی تست شده و ثابت شده است که جایگزین مناسبی برای شبکه ارتباطی مبتنی بر فیبری است که سعی می کند پا به پای رشد ترافیک ادامه پیدا کند.
#
You have been charged with deciding the layout of the new communications network.

شما عهده دار تصمیم گیری در مورد طرح شبکه ارتباطی جدید هستید
#
The current communications network consists of a set of nodes (which route messages), and links of fiber, each of which connects two different nodes.

شبکه ارتباطی فعلی شامل مجموعه ای از گره ها است (که پیام ها رامسیریابی می کند)، و ارتباطات فیبری، که هر یک دو گره متفاوت را بهم متصل می کند
#
For each pair of nodes, there exists at least one way (but possibly more, for bandwidth purposes) to travel along the fiber between the two.

برای هر جفت از گره ها، حداقل یک راه موجود است ( اما احتمالا بیشتر، برای اهداف پهنای باند) برای انتقال از طریق فیبر در بین دو گره
#









The new communications network will not have any fiber.Instead, it will have wireless links, each connecting two nodes.

شبکه ارتباطی جدید هیچ فیبری نخواهد داشت. در عوض، لینک های بی سیم، هر جفت از گره ها را متصل می کند.
#
These links have unbounded bandwidth but are expensive, so it has been decided that as few of these links will be built as possible to provide connectivity.

این لینک ها محدودیت پهنای باند ندارند اما پر خرج و گران هستند، بنابرین تصمیم گرفته شده است که تعداد کمی از این لینک ها برای ایجاد امکان اتصال به اینترنت ساخته شوند.
#
for each pair of nodes there should be exactly one way to travel between them along the wireless links.

برای هر جفت گره باید دقیقا یک راه برای انتقال بین آنها از طریق لینک های بی سیم باشد.
#
Moreover, you discovered that the nodes have each been built with a particular number of connections in mind.

علاوه بر این، شما متوجه شدید که گره ها با تعداد خاصی از اتصالات ساخته شده اند.
#
For each node, if it will be connected to a different number of links than it is today, it will have to be reorganized, and that is costly.

برای هر گره، اگر به تعداد دیگری از لینک ها متصل شود ، باید مجددا سازماندهی شود، و این هزینه بر است.
#
Your task is to design the new network so that it has precisely one path between each pair of nodes while minimizing the number of nodes that do not have the same number of connections as in the original network. 

وظیفه شما این است که شبکه جدیدی را طراحی کنید به طوری که دقیقا یک مسیر بین هر جفت گره باشد و تعداد گره هایی که شماره آنها در شبکه اصلی یکسان است حداقل باشد.
#
Figure 1 shows the original network and a solution for Sample Input 1.

شکل 1 شبکه اصلی و یک راه حل را برای نمونه ورودی 1 را نشان می دهد.

# Input

# ورودی

The input begins with a line containing two integers n (2≤n≤104) and m (1≤m≤105)

ورودی با خطی مشتمل بر دو عدد صحیح آغاز می شود n (2≤n≤104) and m (1≤m≤105)
#
 denoting the number of nodes and the number of fiber links in the existing network.

نشان دهنده تعداد گره ها و تعداد پیوندهای فیبر موجود در شبکه  است.
#
The nodes are numbered from 0 to n−1. 

گره ها ار 0 تا n-1 شمارگذاری شده اند.
#
Each of the next m lines contains two distinct integers ai and bi,

هر خط بعدی m شامل دو عدد صحیح متمایز ai و bi است
#
denoting the fact that the ith fiber link connects nodes numbered ai and bi.

نشان دهنده این واقعیت است که لینک فیبر iام گره های شماره ai و bi را بهم متصل می کند.
#
It is guaranteed that for each pair of nodes there exists at least one path connecting the two nodes. 

تضمین شده است که برای هر جفت گره حداقل یک مسیر وجود دارد که دو گره را متصل می کند.
#
Any pair of nodes may have more than one fiber link connecting them.

هر جفت گره ممکن است دارای بیش از یک پیوند فیبر باشد که آنها را بهم متصل کند.
# Output
# خروجی

Display the smallest number of nodes for which the number of connected links needs to change.

کوچکترین تعداد گره ها را که تعداد لینک های متصل آن نیاز به تغییر دارد را نمایش می دهد.
#
Starting on the next line, display a system of connections in the same format as the input.

در آغاز خط بعد، سیستمی از لینک ها را در همان قالب مشابه ورودی نمایش می دهد.

#
That is, display a line containing the number of nodes (this will be the same as in the input)  and the number of wireless links,  and then on subsequent lines descriptions of the links.

یعنی، یک خط حاوی تعداد گره ها را نمایش می دهد ( درست مشابه ورودی خواهد بود) و تعداد لینک های بی سیم، و سپس در خطوط بعدی توصیف لینک ها.
#
 If more than one layout is possible, any valid layout will be accepted.
اگر بیش از یک طرح بندی امکان پذیر باشد، هر طرح بندی معتبر دیگری هم قابل قبول است.
