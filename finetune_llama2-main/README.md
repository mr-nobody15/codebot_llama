# Fine-tuning LLAMA-2 model using instruct-based dataset
Fine-tuning defines the computational method of downstreaming a pre-trained language model to a domain-specific custom model eventually adjusting the model's parameters to trainable parameters utilized later on. The instruct-based dataset consists of a list of dictionaries of instruction and its respective output. Here the dataset defines the programming-based question and answer in code.

# Applications of Fine-tuning
Fine-tuning pre-trained models are used as enterprise models that can be integrated into the small-scale organization's mainframe application which can be an assistant to their domain-specific application. It can also be used as a step of transfer learning to create a multi-purpose model or more of a multi-model that can do image processing, text generation, and other tasks, etc.

# Lora and Qlora
A heavy computational task like fine-tuning requires a lot of computational memory and resources to train all the parameters, leading to more inference time and memory-inefficient. Lora (Low-ranking Adaption) a method under the PEFT (Parameter Efficient Fine-tuning) injects low-ranking matrices onto the transformer layer preserving the performance of the base model and reducing the number of trainable parameters to avoid the extra computational burden.

QLora (Quantized Lora), is an extension to Lora with the additional introduction of using a normalized floating bit of 4-bits (NF-4) and double quantization to further reduce the memory footprint of training and inference. QLoRA is a versatile technique applicable to different language models, including RoBERTa, DeBERTa, GPT-2, GPT-3, GPT-4, etc.

![image](https://github.com/mr-nobody15/codebot_llama/assets/70313481/63a0a13c-f141-46f3-9a1a-01ef429a3d79)


# Hugging Face repo for QLora Adaptors configuration, tokenizers, and other files link

https://huggingface.co/Akil15/finetune_llama_v_0.1
