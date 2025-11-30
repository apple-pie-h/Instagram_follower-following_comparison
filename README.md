# Instagram Follower & Following Comparison

This repository contains a Jupyter Notebook (`.ipynb`) that helps you compare your Instagram **followers** and **following** using data exported from Instagram/Meta. It generates clear CSV files showing:

* **Common accounts** (people you follow and who follow you back)
* **Follower differences** (people who follow you but you don't follow back)
* **Following differences** (people you follow but who don't follow you back)

---

## 🔧 How to Export Your Instagram Data

Follow these steps to download the required JSON files:

1. **Open Instagram** and go to your profile.
2. Go to **Settings → Accounts Center**.
3. Open **Your information & permissions**.
4. Tap **Download your information**.
5. Select **Create export** → **Export to device**.
6. Choose **Customize information**.
7. Scroll to the **Connections** section.
8. Select **Followers** and **Following** only.
9. Go back once and set **Date Range** to **All time**.
10. Go back again and set **Format** to **JSON**.
11. Download the ZIP file once it's ready.
12. Unzip it and locate the two JSON files:

* `followers.json`
* `following.json`

*A sample format of these files is included in this repository for reference.*

---

## 🧪 How to Use the Notebook

1. Open the `.ipynb` file in Jupyter Notebook, JupyterLab, or Google Colab.
2. Upload your downloaded **followers.json** and **following.json** files.
3. Run all cells in the notebook.

The notebook will parse the JSON files, extract the usernames, compare the lists, and generate output CSV files.

---

## 📁 Output Files

After running the notebook, the following files will be created:

### **1. `common.csv`**

Contains accounts that appear in **both** lists — people you follow *and* who follow you back.

### **2. `follower_diff.csv`**

Contains usernames who **follow you**, but **you do NOT follow back**.

### **3. `following_diff.csv`**

Contains usernames you **follow**, but **they do NOT follow you back**.

---

## ✔️ Notes

* The script only works with **JSON** files exported from Meta.
* Ensure your files strictly match Instagram's export format.
* If your exported files have names like `followers_1.json` or `following_1.json`, please **rename them** to `followers.json` and `following.json`, or **update the filenames directly in the notebook code** before running.
* If the structure changes in future Meta updates, the parsing may need to be adjusted.

---

## 📬 Questions or Issues?

Feel free to open an issue or reach out if something isn't working correctly!
