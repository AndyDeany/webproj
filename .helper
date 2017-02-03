import os
html = []
for item in os.listdir(os.getcwd()):
    if item[-5:] == ".html" and item != "index.html":
        html.append(item[:-5])
        old = open(item, "r")
        new = open(item + ".tmp", "w")
        for line in old:
            line = line.replace(
                "E:\\Users\\Andrew\\Desktop\\Websites\\hip-prop.co.uk\\working\\",
                "http://hip-prop.co.uk/"
                )
            new.write(line.replace(".html", "/"))
        old.close()
        new.close()
        os.remove(item)
        os.rename(item + ".tmp", item)
                      

for page in html:    
    os.mkdir(page)
    os.rename(page + ".html", page + "/index.html")
