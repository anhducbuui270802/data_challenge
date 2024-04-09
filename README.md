# UIT Data_challenge 2023
Recent developments of modern chatbot systems such as ChatGPT of OpenAI or BARD of Google have raised concerns about the information validity they provide. Information checking has therefore become a crucial part and must be integrated into any modern chatbot system in order to provide reliable information for users.

![requirement](ICHEVE.png)

In this challenge, participants will take part in an information-checking task. In particular, we provide ISE-DSC01, a dataset containing various claims and appropriate texts. Participants have to develop methods to verify claims given their texts.

The ISE-DSC01 has 48,000+ samples. Each sample includes a claim and context. Participants have to propose a method to verify the claims using information of the given context. That is determine whether that claim is SUPPORTED given context, or REFUTED given context, or NEI (Not Enough Information) if the given context can not support or refute the claim.

In case of pointing out the given claim is SUPPORTED or REFUTED, proposed methods have to extract exactly one sentence from context as evidence. There is no need to provide evidence for NEI claim.

ISE-DSC01 dataset is saved in JSON format and structured as follows:

{

     “id”:

          {

             ”context”: “văn phòng quận yongsan, trung tâm thủ đô … ”,

             “claim”: “xấp xỉ một triệu khách du lịch đã đến Hàn Quốc mỗi năm vì lễ hội ẩm thực toàn cầu”,

            “verdict”: “SUPPORTED”,

            “evidence”: “văn phòng quận cũng sẽ thực hiện …”

         },

         …

}

Training and Public Test set: https://drive.google.com/drive/folders/16emQgeEm6OsF95rDV7nwlrBvBP8uCW5m?usp=share_link.

Private Test set: https://drive.google.com/drive/folders/1tK3992az51JA0wuGyg40ItgrJ4boxAQf?usp=share_link.