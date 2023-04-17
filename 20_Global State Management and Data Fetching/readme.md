1. Redux
    - Redux adalah library untuk manajemen state global. Redux menggunakan struktur "one-way data flow". Redux menggunakan beberapa type code.
    - Saat yang tepat untuk menggunakan redux adalah:
        - Banyak state yang perlu ditaruh dibanyak tempat
        - State pada aplikasi sering berubah
        - Logic untuk mengubah state kompleks
        - Ukuran codebase yang sedang-besar, dan dikerjakan oleh banyak orang
        - Perlu mengetahui bagaimana state diupdate seiring dengan waktu
    - Berikut Redux libraries dan tools:
        - React Redux, cara termudah untuk berkomunikasi dengan redux dari komponen react
        - Redux Toolkit, berisi package dan function untuk membuat store redux
        - Redux Devtools Extension, digunakan untuk melihat history state sehingga mudah untuk melakukan debugging
    - Beberapa komponen penting redux, yakni:
        - Actions, ibarat parameter dengan isinya type data rata-rata string. Digunakan untuk memberikan informasi dari aplikasi ke store
        - Reducer, adalah pure javascript functions yang mengambil state aplikasi saat ini dan object action lalu mengembalikan state aplikasi terbaru
        - Store, adalah objek sentral yang menyimpan state pada aplikasi
    - Ada 2 cara memakai dan mengubah state pada redux store
        - Hooks
        - Connect

2. Redux Thunk
    - Redux Thunk adalah Thunk middleware untuk redux yang memungkinkan kita untuk membuat action creator yang mengembalikan function bukan action
    - Alasan kita perlu menggunakan redux-thunk adalah untuk menghandle side effect logic seperti logic synchronous kompleks yang perlu mengakses store dan juga logic asyncrhonous seperti request data

3. Fetching Data
    - Fetching Data adalah proses pengambilan perintah dan data yang diperlukan.
    - Beberapa cara untuk fetching data di react:
        - Fetch API
        - Axios
        - React Query Library