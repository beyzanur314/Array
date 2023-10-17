
struct Account yapısı: Bu yapı, adminlerin bilgilerini içerecek şekilde tanımlanabilir.

Account[] public admins;: admins adında bir Account türünden dinamik bir dizi oluşturuldu. Bu dizi, admin hesaplarını depolamak için kullanılır.

function addAdmin(Account memory newAdmin) public: Bu fonksiyon, yeni bir admin eklemek için kullanılır. Fonksiyon, newAdmin adında bir Account yapısını kabul eder ve bu yapıyı admins dizisine ekler.

function getAllAdmins() public view returns (Account[] memory): Bu fonksiyon, tüm admin hesaplarını döndürmek için kullanılır. Dinamik bir dizi olan admins dizisini döndürür.

function getAllAdminsFixed() public view returns (Account[3] memory): Bu fonksiyon, sabit bir dizi olarak en fazla 3 admin hesabını döndürmek için kullanılır. admins dizisinde en az 3 admin hesabı olması gerekmektedir; aksi takdirde bir hata fırlatır.
