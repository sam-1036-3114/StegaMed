# StegaMed

### **A Python-based Steganography Tool for Securing Medical Information**

StegaMed is a project that implements steganography to securely embed medical reports into images. This ensures that sensitive medical information remains hidden yet accessible when needed.

---

## Features

- 🔒 **Secure Medical Data Embedding**: Uses the Least Significant Bit (LSB) technique to hide medical information in images.
- 🖼️ **Supports PNG Images**: Works with lossless `.png` image format for data integrity.
- 📜 **Medical Report Handling**: Embeds structured medical reports in JSON format.
- 🔍 **Data Extraction**: Retrieves hidden information seamlessly without altering the original data.

---

## Use Cases

- **Healthcare**: Securely share patient records with embedded medical data in diagnostic images.
- **Data Security**: Protect sensitive information in plain sight.

---

## How It Works

1. **Prepare Input Image**:
   - Upload a `.png` file as the cover image for embedding data.
2. **Medical Report**:
   - The tool encodes a medical report (in JSON format) into the image's pixel values.
3. **Embedding**:
   - Encodes data into the least significant bits (LSBs) of pixel values.
4. **Extraction**:
   - Retrieves the embedded medical information without visual degradation.

---

## Requirements

- **Python 3.8+**
- Libraries:
  - `Pillow`: For image processing.
  - `matplotlib`: For image visualization (optional in Colab).

Install the required libraries using:
```bash
pip install pillow matplotlib
How to Use
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/yourusername/StegaMed.git
cd StegaMed
2. Run the Program
Use the provided Python script to embed or extract data:

bash
Copy
Edit
python steganography.py
3. In Google Colab
Upload steganography.ipynb to your Colab workspace.

Execute the notebook for embedding and extracting data.

File Structure
plaintext
Copy
Edit
StegaMed/
│
├── steganography.py       # Main Python script
├── medical_report.json    # Sample medical report
├── input.png              # Example input image
├── README.md              # Project documentation
└── requirements.txt       # Required libraries
Sample Medical Report
json
Copy
Edit
{
  "patient_id": "123456",
  "name": "John Doe",
  "age": 35,
  "gender": "Male",
  "diagnosis": "Hypertension",
  "prescription": [
    {"medicine_name": "Amlodipine", "dosage": "5 mg", "frequency": "Once daily"},
    {"medicine_name": "Hydrochlorothiazide", "dosage": "25 mg", "frequency": "Once daily"}
  ],
  "tests_recommended": ["Blood Pressure Monitoring", "Kidney Function Test"]
}
Output Example
Input Image: input.png

Output Image: output.png (with embedded data)

Extracted Data: Displays the original medical report.

Contributing
Contributions are welcome! Please fork this repository and submit a pull request with your enhancements.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Contact
For queries or collaboration:

Email: sambasivaraogandikota052@gmail.com

GitHub: sam-1036-3114

yaml
Copy
Edit

---

Let me know if you'd like help with uploading this file or customizing it further!