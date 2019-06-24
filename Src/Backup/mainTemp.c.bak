/**
  ******************************************************************************
  * File Name          : main.c
  * Description        : Main program body
  ******************************************************************************
  *
  * COPYRIGHT(c) 2016 STMicroelectronics
  *
  * Redistribution and use in source and binary forms, with or without modification,
  * are permitted provided that the following conditions are met:
  *   1. Redistributions of source code must retain the above copyright notice,
  *      this list of conditions and the following disclaimer.
  *   2. Redistributions in binary form must reproduce the above copyright notice,
  *      this list of conditions and the following disclaimer in the documentation
  *      and/or other materials provided with the distribution.
  *   3. Neither the name of STMicroelectronics nor the names of its contributors
  *      may be used to endorse or promote products derived from this software
  *      without specific prior written permission.
  *
  * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
  * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
  * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
  * DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
  * FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
  * DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
  * SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
  * CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  *
  ******************************************************************************
  */
/* Includes ------------------------------------------------------------------*/
#include "stm32f1xx_hal.h"
#include "i2c.h"
#include "usart.h"
#include "gpio.h"

/* USER CODE BEGIN Includes */
#include "fonts.h"
#include "ssd1306.h"
/* USER CODE END Includes */

/* Private variables ---------------------------------------------------------*/

/* USER CODE BEGIN PV */
/* Private variables ---------------------------------------------------------*/

/* USER CODE END PV */

/* Private function prototypes -----------------------------------------------*/
void SystemClock_Config(void);

/* USER CODE BEGIN PFP */
/* Private function prototypes -----------------------------------------------*/

/* USER CODE END PFP */

/* USER CODE BEGIN 0 */


/* USER CODE END 0 */

int main(void)
{
int time = 25;
int counter = 2;
int temp = 25;
int humd = 40;
char str[3];
int day=19;
int mon = 06;
int yer=19;
int now=54000;
	int graph[80];
	
  /* USER CODE BEGIN 1 */

  /* USER CODE END 1 */

  /* MCU Configuration----------------------------------------------------------*/

  /* Reset of all peripherals, Initializes the Flash interface and the Systick. */
  HAL_Init();

  /* Configure the system clock */
  SystemClock_Config();

  /* Initialize all configured peripherals */
  MX_GPIO_Init();
  MX_I2C1_Init();
  MX_USART1_UART_Init();

  /* USER CODE BEGIN 2 */
	uint8_t res = SSD1306_Init();
//SSD1306_GotoXY(0, 44);


//print animation
SSD1306_Fill(SSD1306_COLOR_BLACK);
SSD1306_UpdateScreen();
HAL_Delay(time);
for (int i = 0; i < 35; i++)
{
		SSD1306_DrawFilledCircle(64, 32, i*2, SSD1306_COLOR_WHITE);
	SSD1306_UpdateScreen();
HAL_Delay(time);
}
for (int i = 0; i < 30; i++)
{
		SSD1306_DrawFilledCircle(64, 32, i*2, SSD1306_COLOR_BLACK);
	SSD1306_UpdateScreen();
HAL_Delay(time);
}
for (int i = 0; i < 25; i++)
{
		SSD1306_DrawFilledCircle(64, 32, i*2, SSD1306_COLOR_WHITE);
	SSD1306_UpdateScreen();
HAL_Delay(time);
}
for (int i = 0; i < 20; i++)
{
		SSD1306_DrawFilledCircle(64, 32, i*2, SSD1306_COLOR_BLACK);
	SSD1306_UpdateScreen();
HAL_Delay(time);
}
for (int i = 0; i < 15; i++)
{
		SSD1306_DrawFilledCircle(64, 32, i*2, SSD1306_COLOR_WHITE);
	SSD1306_UpdateScreen();
HAL_Delay(time);
}
for (int i = 0; i < 35; i++)
{
		SSD1306_DrawFilledCircle(64, 32, i*2, SSD1306_COLOR_BLACK);
	SSD1306_UpdateScreen();
HAL_Delay(time);
}



while(1)
{
temp += rand ()%3;
	temp -= rand()%3;
	humd += rand()%3;
	humd -= rand()%3;
//print symbols
SSD1306_Fill(SSD1306_COLOR_BLACK);
SSD1306_DrawPixel(11, 10, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(10, 11, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(11, 11, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(12, 11, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(10, 12, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(11, 12, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(12, 12, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(10, 13, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(11, 13, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(12, 13, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(10, 14, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(11, 14, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(12, 14, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(10, 15, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(11, 15, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(12, 15, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(10, 16, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(11, 16, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(12, 16, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(9, 17, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(10, 17, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(11, 17, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(12, 17, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(13, 17, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(9, 18, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(10, 18, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(11, 18, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(12, 18, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(13, 18, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(10, 19, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(11, 19, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(12, 19, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(11, 20, SSD1306_COLOR_WHITE);




SSD1306_DrawFilledCircle(10, 25, 1, SSD1306_COLOR_WHITE);
SSD1306_DrawFilledCircle(10, 29, 1, SSD1306_COLOR_WHITE);
SSD1306_DrawFilledCircle(14, 27, 1, SSD1306_COLOR_WHITE);
SSD1306_DrawFilledCircle(14, 31, 1, SSD1306_COLOR_WHITE);


	
//print bars
SSD1306_DrawRectangle(28, 10, 65, 5, SSD1306_COLOR_WHITE);
SSD1306_DrawFilledRectangle(28, 10, temp, 5, SSD1306_COLOR_WHITE);
	
SSD1306_DrawRectangle(28, 25, 65, 5, SSD1306_COLOR_WHITE);
SSD1306_DrawFilledRectangle(28, 25, humd, 5, SSD1306_COLOR_WHITE);

SSD1306_DrawPixel(28, 10, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(29, 10, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(28, 9, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(29, 9, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(28, 8, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(29, 8, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(28, 7, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(29, 7, SSD1306_COLOR_WHITE);

SSD1306_DrawPixel(92, 10, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(93, 10, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(92, 9, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(93, 9, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(92, 8, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(93, 8, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(92, 7, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(93, 7, SSD1306_COLOR_WHITE);

SSD1306_DrawPixel(48, 10, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(49, 10, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(48, 9, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(49, 9, SSD1306_COLOR_WHITE);

SSD1306_DrawPixel(78, 10, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(79, 10, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(78, 9, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(79, 9, SSD1306_COLOR_WHITE);



SSD1306_DrawPixel(28, 25, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(29, 25, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(28, 24, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(29, 24, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(28, 23, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(29, 23, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(28, 22, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(29, 22, SSD1306_COLOR_WHITE);

SSD1306_DrawPixel(92, 25, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(93, 25, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(92, 24, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(93, 24, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(92, 23, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(93, 23, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(92, 22, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(93, 22, SSD1306_COLOR_WHITE);

SSD1306_DrawPixel(48, 25, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(49, 25, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(48, 24, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(49, 24, SSD1306_COLOR_WHITE);

SSD1306_DrawPixel(78, 25, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(79, 25, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(78, 24, SSD1306_COLOR_WHITE);
SSD1306_DrawPixel(79, 24, SSD1306_COLOR_WHITE);



	
//print values
SSD1306_GotoXY(100,8);
sprintf(str, "%d", temp);
str[2]='C';
SSD1306_Puts(str, &Font_7x10, SSD1306_COLOR_WHITE);
	
SSD1306_GotoXY(100,22 );
sprintf(str, "%d", humd);
str[2]='%';
SSD1306_Puts(str, &Font_7x10, SSD1306_COLOR_WHITE);
	
//print time
now++;
/*
SSD1306_GotoXY(20,45);
sprintf(str, "%d", now/3600);

str[2]=':';
SSD1306_Puts(str, &Font_11x18, SSD1306_COLOR_WHITE);
SSD1306_GotoXY(60,45);
str[0]=' ';
str[1]=' ';
sprintf(str, "%d", now/60);

str[2]=' ';
SSD1306_Puts(str, &Font_11x18, SSD1306_COLOR_WHITE);
*/



//print graph
if (now < 80) graph[now] = 80-temp;
else now = 0;

for(int i=0; i < 80; i++)
{
	SSD1306_DrawPixel(20+i, graph[i], SSD1306_COLOR_WHITE);
}

HAL_Delay(500);
SSD1306_UpdateScreen();
}
}

/** System Clock Configuration
*/
void SystemClock_Config(void)
{

  RCC_OscInitTypeDef RCC_OscInitStruct;
  RCC_ClkInitTypeDef RCC_ClkInitStruct;

  RCC_OscInitStruct.OscillatorType = RCC_OSCILLATORTYPE_HSE;
  RCC_OscInitStruct.HSEState = RCC_HSE_ON;
  RCC_OscInitStruct.HSEPredivValue = RCC_HSE_PREDIV_DIV1;
  RCC_OscInitStruct.PLL.PLLState = RCC_PLL_ON;
  RCC_OscInitStruct.PLL.PLLSource = RCC_PLLSOURCE_HSE;
  RCC_OscInitStruct.PLL.PLLMUL = RCC_PLL_MUL9;
  HAL_RCC_OscConfig(&RCC_OscInitStruct);

  RCC_ClkInitStruct.ClockType = RCC_CLOCKTYPE_HCLK|RCC_CLOCKTYPE_SYSCLK
                              |RCC_CLOCKTYPE_PCLK1|RCC_CLOCKTYPE_PCLK2;
  RCC_ClkInitStruct.SYSCLKSource = RCC_SYSCLKSOURCE_PLLCLK;
  RCC_ClkInitStruct.AHBCLKDivider = RCC_SYSCLK_DIV1;
  RCC_ClkInitStruct.APB1CLKDivider = RCC_HCLK_DIV2;
  RCC_ClkInitStruct.APB2CLKDivider = RCC_HCLK_DIV1;
  HAL_RCC_ClockConfig(&RCC_ClkInitStruct, FLASH_LATENCY_2);

  HAL_SYSTICK_Config(HAL_RCC_GetHCLKFreq()/1000);

  HAL_SYSTICK_CLKSourceConfig(SYSTICK_CLKSOURCE_HCLK);

  /* SysTick_IRQn interrupt configuration */
  HAL_NVIC_SetPriority(SysTick_IRQn, 0, 0);
}

/* USER CODE BEGIN 4 */

/* USER CODE END 4 */

#ifdef USE_FULL_ASSERT

/**
   * @brief Reports the name of the source file and the source line number
   * where the assert_param error has occurred.
   * @param file: pointer to the source file name
   * @param line: assert_param error line source number
   * @retval None
   */
void assert_failed(uint8_t* file, uint32_t line)
{
  /* USER CODE BEGIN 6 */
  /* User can add his own implementation to report the file name and line number,
    ex: printf("Wrong parameters value: file %s on line %d\r\n", file, line) */
  /* USER CODE END 6 */

}

#endif

/**
  * @}
  */ 

/**
  * @}
*/ 

/************************ (C) COPYRIGHT STMicroelectronics *****END OF FILE****/
