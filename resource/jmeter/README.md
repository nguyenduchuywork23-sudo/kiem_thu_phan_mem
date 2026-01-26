# JMeter Performance Test Report

## Muc tieu
- Hieu cach su dung JMeter de kiem thu hieu nang.
- Thiet ke kich ban kiem thu voi tham so khac nhau.
- Phan tich ket qua va viet bao cao.

## Website duoc kiem thu
- URL: https://en.wikipedia.org

## Moi truong
- JMeter version: 5.6.3
- OS: Windows

## Cau hinh va kich ban
HTTP Request Defaults
Protocol: https
Server Name: en.wikipedia.org
HTTP Header Manager
User-Agent: Custom (tránh lỗi HTTP 403)
Listeners
Summary Report
View Results Tree

### Thread Group 1 (Basic)
Number of Threads: 10
Loop Count: 5
Request:
GET /

### Thread Group 2 (Heavy)
Number of Threads: 50
Ramp-up Period: 30 giây
Requests:
GET /
GET /wiki/Main_Page

### Thread Group 3 (Custom)
Number of Threads: 20
Duration: 60 giây (Scheduler)
Requests:
GET /wiki/1
GET /wiki/2

## Ket qua (trich tu Summary Report)
| Label       | Avg Response Time (ms) | Throughput (req/sec) | Error %  |
| ----------- | ---------------------- | -------------------- | -------- |
| GET_Home    | 2607                   | 1.41                 | 0.00     |
| GET_Subpage | 1817                   | 1.47                 | 0.00     |
| GET_1       | 4788                   | 2.27                 | 0.00     |
| GET_2       | 2877                   | 2.28                 | 0.00     |
| **TOTAL**   | **2657**               | **1.79**             | **0.00** |

- File ket qua: `results/summary.csv`

## Minh chung
# <img src="resource/images/Screenshot 2026-01-26 092745.png" width="100%" alt="Bài Tập Chương 2">
# <img src="resource/images/Screenshot 2026-01-26 092711.png" width="100%" alt="Bài Tập Chương 2">
# <img src="resource/images/Screenshot 2026-01-26 092638.png" width="100%" alt="Bài Tập Chương 2">
# <img src="resource/images/Screenshot 2026-01-26 092552.png" width="100%" alt="Bài Tập Chương 2">