# DE-Project02BeautifulSoup

Bài toán: Sau khi bitcoin và các đồng tiền ảo sụt giảm, công ty có nhu cầu khảo sát thông tin về card đồ họa thông qua một website. Yêu cầu team Data Engineer collect và thống kê các thông tin tại danh mục trên website: [https://www.newegg.com](https://www.newegg.com/GPUs-Video-Graphics-Cards/SubCategory/ID-48?Tid=7709) để phía đội kinh doanh có cơ sở triển khai chiến dịch mới.

Mô tả cụ thể:

- Nguồn dữ liệu cần crawl là danh mục sau: https://www.newegg.com/GPUs-Video-Graphics-Cards/SubCategory/ID-48?Tid=7709
- Thông tin cần lấy:
    - ItemID
    - Title
    - Branding (Hãng)
    - Rating
    - Số lượng Rating
    - Price (Current Price) → Chuyển đổi dưới dạng number
    - Shipping (Free, Ko ship, hay mất phí)
    - Image URL
    - Các thông tin chi tiết về sản phẩm:
        -- Max Resolution
        -- DisplayPort
        -- HDMI
        -- DirectX
        -- Model
        
        
File: BeautifulSoup_final.ipynb

+ Part 1: scrape data from web and store it to the csv file
-- Scrape data from website and store it to the combined_data dictionary
-- Read the dictionary to the CSV file 'newegg_products.csv'
-- Store the logfile when reading the data in logfile.log 

+ Part 2 :Transform, clean and visualize data
-- Read data from csv file using Pandas library
-- Exploratory analysis: metadata and detecting anomalies ( too many empty variables, duplicates, ...)
-- Transform and clean data
-- Visualize data 

File: db_connection.ipynb
Connect to the SQL database 'unigap_de_p02' and read the csv file ''newegg_products.csv' as table