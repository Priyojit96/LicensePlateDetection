# LicensePlateDetection
A simple License Plate Detection using Open CV and EasyOCR. My system was made in accordance to European Conditions. You can change according to Indian Conditions by changing the 2D array part.
text = result[1][-2]

font = cv2.FONT_HERSHEY_SIMPLEX
res = cv2.putText(img, text=text, org=(approx[0][0][0], approx[1][0][1]+60), fontFace=font, fontScale=1, color=(0,255,0), thickness=2, lineType=cv2.LINE_AA)
res = cv2.rectangle(img, tuple(approx[0][0]), tuple(approx[2][0]), (0,255,0),3)
plt.imshow(cv2.cvtColor(res, cv2.COLOR_BGR2RGB))

Here you can change the system by changing the array number in the text line for your own requirement. My system is observed and works well in a normal day condition without rain and sunglare which are yet to be tested.

Find the current system on Google colab with this link: https://colab.research.google.com/drive/1dQ-fnYjJ6bGNkcACcth9u2uWWzymzk5r?usp=sharing
