# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Model based clustering Use Mclust (mclust) With (In) R Software
install.packages("mclust")
library("mclust")
Mclust = read.csv("https://raw.githubusercontent.com/timbulwidodostp/Mclust/main/Mclust/Mclust.csv",sep = ";")
# Estimation Model based clustering Use Mclust (mclust) With (In) R Software
Mclust_1 = Mclust(Mclust[,1:4])
summary(Mclust_1)
Mclust_2 = Mclust(Mclust[,1:4], G = 1)
summary(Mclust_2)
Mclust_3 = Mclust(Mclust[,1:4], prior = priorControl())
summary(Mclust_3)
Mclust_4 = Mclust(Mclust[,1:4], prior = priorControl(functionName="defaultPrior", shrinkage=0.1))
summary(Mclust_4)
# Model based clustering Use Mclust (mclust) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished